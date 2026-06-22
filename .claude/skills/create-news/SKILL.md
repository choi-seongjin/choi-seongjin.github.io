---
name: create-news
description: Draft a lab-website news post from recent publication/site changes, then notify for review. Use when the user says "create news," "create a news post," "draft news," "announce this paper," "create news autonomously," or after a paper is accepted/published or the publications list changes. Draft-only — never auto-publishes to the live site.
---

# Create News Skill

Generates a news post for the Choi Lab website (`choi-seongjin.github.io`) in the
house style, from recent changes — **and stops at a draft for human review.**

## Autonomy boundary (HARD RULE)
- **Draft + notify only.** Write the post to `_drafts/`, then report the draft path
  and a summary to the user. **Never** write to `_posts/`, **never** `git commit`,
  **never** `git push`. Publishing is a human action (move `_drafts/<file>` → `_posts/`).
- Rationale: news is public-facing and metadata is error-prone. Real cases caught by
  review: a paper's title silently changed on arXiv; a co-author was missing; an entry
  said "in press" when it was already published with a DOI; a venue claim was unverifiable.
  An auto-publisher would have shipped all of these. Detect and draft; let a human verify.

## Triggers / sources (use BOTH)
Primary — **publication-list git diffs**:
- `git -C <repo> log -p -- pages/quiet-publications.md` and `git diff` for uncommitted edits.
- Newsworthy signals in `<article class="pub-entry">` blocks:
  - a **new** entry added;
  - `data-type` flips `preprint`/`conference` → `journal` (acceptance / in press);
  - meta gains a **volume/article number** or a **DOI ↗** link (now published);
  - `(in press)` removed from the meta (now published).
- Other site changes worth a post: new team members (`pages/quiet-team.md`), talks, awards,
  funded grants, released data/code.

Enrichment — **Claude Code chat logs** (context only, never the sole source):
- Project transcripts: `/data/chois/.claude/projects/-data-chois-active-choi-seongjin-github-io/*.jsonl`.
- Use to recover *why*/*what* (e.g. the user said "X is in press at Y", a DOI was pasted).
- Treat as hints; **verify every fact against the publications page or an authoritative source**
  before putting it in a draft.

## Workflow
1. **Collect changes.** Diff `pages/quiet-publications.md` (committed history + working tree).
   Skim recent chat transcripts for matching context.
2. **Cluster into a story.** Group related items (e.g. "three new papers"). One post can
   feature multiple papers.
3. **Verify metadata** for each item before writing — venue, volume, article no., DOI, and the
   **full ordered author list**. Use the `refcheck` skill / `WebSearch` / `WebFetch` (arXiv,
   publisher page). Distinguish **published** (has DOI/volume) from **in press / accepted**
   (no DOI yet). Use full author first names (cross-check `pages/quiet-team.md`).
4. **Draft** the post (template below) into `_drafts/`.
5. **Notify.** Report: the draft file path, a one-line summary of each featured item, any
   facts you could **not** verify (flag explicitly), and the exact command to publish:
   `git mv _drafts/<file> _posts/<file>`.

## House style (match existing `_posts/`)
- **Filename:** `_drafts/YYYY-MM-DD-<slug>.md` (today's date). Publishing moves it to `_posts/`.
- **Frontmatter:**
  ```yaml
  ---
  layout: page-fullwidth
  title: "<concise descriptive title>"
  meta_title: ""
  subheadline: "Publications"          # or "Talk", "People", "Award", etc.
  teaser: "<1–2 sentence summary; accurate on published vs in-press>"
  permalink: "/news/YYMMDD"            # 6-digit date code, e.g. 260620
  header: no
  readmore: true                        # true when there is body text; false for teaser-only
  ---
  ```
- **Body:** Markdown. First person ("I'm excited to share…"). For each paper: **bold title**,
  the venue (italic *journal name*; add Volume/Article when published), full author names in
  **bold** for lab members, 1–3 sentences of plain-language summary (do **not** over-claim
  beyond what's verified), then a link line (`📄 [DOI: … ↗](https://doi.org/…)` or
  `📄 [arXiv:… ↗](https://arxiv.org/abs/…)`). Close with a short congratulations line.
- **Accuracy:** say "published in *X* (Volume, Article)" only with a DOI/volume; otherwise
  "accepted and is in press at *X*". Never invent author first names, DOIs, or volumes.

## Example (reference)
See `_posts/2026-06-20-three-new-papers.md` — three items (one published TR-C with DOI,
two in press) in the correct house style.

## Later: scheduling (cron) — deferred until drafts are trusted
Once the user trusts these drafts, wrap this skill in a scheduled cloud agent via the
`/schedule` skill (e.g. weekly). The scheduled run must keep the **draft + notify** boundary:
detect → verify → write to `_drafts/` → open a PR or notify. It must **not** publish to
`gh-pages` unattended.
