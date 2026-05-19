---
layout: editorial
title: Data & Code
editorial_page: Data & Code
permalink: "/datacode/"
---

<div data-repos-root>
<section class="mono-module" style="min-height:calc(100vh - 240px);">
  <div class="terminal-bar">
    <span>// system:brut · page = /datacode</span>
    <span class="progress">▮▮▮▮▮▮▮▮▯▯ &nbsp; reproducibility in progress</span>
    <span>chois@umn:~/lab$ ls -la</span>
  </div>

  <div class="mono-hero">
    <div>
      <p class="kicker kicker-mark">Lab notebook · code &amp; data</p>
      <h1 class="big">REPOS &amp;<br/><span class="accent">DATASETS.</span></h1>
      <p>// Every featured paper ships with a repo and, where licensable, a dataset.<br/>
         // Stars + last-commit pulled at build time. No live API calls — pages stay fast.<br/>
         // If a paper is missing from this list, the code is private or pending release; open an issue and we'll surface it.</p>
    </div>
    <div class="side-card">
      <div class="ls-head">$ ls | wc -l</div>
      <div class="ls-row">
        <span>public repos</span><span class="v">3</span>
        <span>public datasets</span><span class="v">2</span>
        <span>active benchmarks</span><span class="v">1</span>
      </div>
      <div class="sep">
        <a href="https://github.com/UMN-Choi-Lab" class="link-underline">github.com/UMN-Choi-Lab ↗</a>
      </div>
    </div>
  </div>

  <!-- REPOS TABLE -->
  <div class="mono-section">
    <div style="display:flex;justify-content:space-between;align-items:baseline;margin-bottom:18px;flex-wrap:wrap;gap:16px;">
      <h2 class="heading">PUBLIC REPOSITORIES</h2>
      <div style="display:flex;gap:6px;flex-wrap:wrap;">
        <button class="chip mono active" data-repo-filter="All">All</button>
        <button class="chip mono" data-repo-filter="GenAI">GenAI</button>
        <button class="chip mono" data-repo-filter="Forecasting">Forecasting</button>
        <button class="chip mono" data-repo-filter="VLA">VLA</button>
        <button class="chip mono" data-repo-filter="LLM">LLM</button>
        <button class="chip mono" data-repo-filter="Trajectories">Trajectories</button>
        <button class="chip mono" data-repo-filter="Dataset">Dataset</button>
      </div>
    </div>

    <div class="repos-table">
      <div class="row head">
        <span>№</span><span>Repository</span><span>Description</span><span>Tags</span><span>Lang</span><span>★ Stars</span><span>Updated</span>
      </div>

      <a href="https://github.com/UMN-Choi-Lab/DGMinTransportation" class="row repo-row naked" data-tags="GenAI">
        <span class="num">01</span>
        <span class="repo">~/UMN-Choi-Lab/DGMinTransportation</span>
        <span class="desc">Companion repository for the TR-C 2025 survey on deep generative models in transportation research — tutorial notebooks and code references.</span>
        <span class="tags">GenAI</span>
        <span>Jupyter</span>
        <span>★ —</span>
        <span class="upd">—</span>
      </a>

      <a href="https://github.com/UMN-Choi-Lab/BO4Mob" class="row repo-row naked" data-tags="Optimization|LLM">
        <span class="num">02</span>
        <span class="repo">~/UMN-Choi-Lab/BO4Mob</span>
        <span class="desc">Bayesian optimization benchmarks for high-dimensional urban mobility problems (NeurIPS 2025 Datasets &amp; Benchmarks).</span>
        <span class="tags">Optimization · LLM</span>
        <span>Python</span>
        <span>★ —</span>
        <span class="upd">—</span>
      </a>

      <a href="https://github.com/benchoi93/TrajGAIL" class="row repo-row naked" data-tags="GenAI|Trajectories">
        <span class="num">03</span>
        <span class="repo">~/benchoi93/TrajGAIL</span>
        <span class="desc">Generating urban vehicle trajectories using generative adversarial imitation learning (TR-C 2021).</span>
        <span class="tags">GenAI · Trajectories</span>
        <span>Python</span>
        <span>★ —</span>
        <span class="upd">—</span>
      </a>

      <div class="repos-empty" style="display:none;padding:36px;margin-top:16px;border:1px dashed var(--mono-sub);text-align:center;color:var(--mono-sub);font-family:var(--mfont);">
        // no repos match that tag
      </div>
    </div>

    <p style="margin-top:18px;font-family:var(--mfont);font-size:12px;color:var(--mono-sub);line-height:1.7;">
      // Canonical list lives at <a href="https://github.com/UMN-Choi-Lab" class="link-underline" style="color:var(--mono-accent);border-color:var(--mono-accent);">github.com/UMN-Choi-Lab ↗</a>.<br/>
      // ★ counts pending — to be cached at build time when a fetch step is wired in.
    </p>
  </div>

  <!-- DATASETS -->
  <div class="mono-section" style="border-top:1px solid var(--mono-line);">
    <h2 class="heading">PUBLIC DATASETS</h2>
    <div class="dataset-grid">
      <div class="dataset-card">
        <div>
          <div class="label-tiny">Dataset</div>
          <div class="name">MTOdata</div>
          <div class="desc">Curated mobility &amp; transportation operations datasets, hosted at mtodata.github.io.</div>
          <div class="meta"><span>—</span><span>license · varies</span><span>cite · per-dataset</span></div>
        </div>
        <a href="https://mtodata.github.io/" class="dl">Open ↗</a>
      </div>
      <div class="dataset-card">
        <div>
          <div class="label-tiny">Dataset</div>
          <div class="name">PeMS-BAY-2022</div>
          <div class="desc">Updated PeMS-BAY traffic-speed dataset (Bay Area, 2022) — a refresh of the widely-used PeMS-BAY benchmark for spatiotemporal forecasting.</div>
          <div class="meta"><span>—</span><span>license · open</span><span>cite · UMN Choi Lab</span></div>
        </div>
        <a href="https://github.com/UMN-Choi-Lab/PeMS-BAY-2022" class="dl">Open ↗</a>
      </div>
    </div>
  </div>

  <!-- HOW TO CITE + REPRO CHECKLIST -->
  <div class="cite-grid">
    <div>
      <h2 class="heading">HOW TO CITE</h2>
      <p>// If you use one of our datasets or a derived benchmark,<br/>
         // please cite the source paper and the dataset record.<br/>
         // BibTeX keys follow <span class="accent" style="color:var(--mono-accent);">author + year + first-word</span>.</p>
      <div class="bib-block" id="bib-example">@article&#123;choi2025dgm,
  title   = &#123;A Gentle Introduction and Tutorial on Deep Generative
             Models in Transportation Research&#125;,
  author  = &#123;Choi, Seongjin and Jin, Zhixiong and Ham, Seung Woo
             and Kim, Jiwon and Sun, Lijun&#125;,
  journal = &#123;Transportation Research Part C: Emerging Technologies&#125;,
  volume  = &#123;176&#125;,
  pages   = &#123;105145&#125;,
  year    = &#123;2025&#125;,
  doi     = &#123;10.1016/j.trc.2025.105145&#125;
&#125;</div>
      <button class="copy-bib" data-target="#bib-example">Copy BibTeX</button>
    </div>

    <div>
      <h2 class="heading">REPRODUCIBILITY CHECKLIST</h2>
      <p>// We commit to the following for every released repo:</p>
      <ul class="repro-list">
        <li><span class="done">[x]</span><span>Pinned dependencies · requirements.txt or environment.yml</span></li>
        <li><span class="done">[x]</span><span>Single-command training entrypoint · scripts/train.sh</span></li>
        <li><span class="done">[x]</span><span>Single-command evaluation · scripts/eval.sh</span></li>
        <li><span class="done">[x]</span><span>Pre-trained checkpoints when license permits</span></li>
        <li><span class="done">[x]</span><span>Dataset DOI or download script</span></li>
        <li><span class="pending">[ ]</span><span class="pending-text">Hardware &amp; wall-clock from the paper (partial)</span></li>
        <li><span class="pending">[ ]</span><span class="pending-text">Hyperparameter search logs (partial)</span></li>
      </ul>
      <p class="repro-foot">
        // Issues for missing artifacts: file at <a href="https://github.com/UMN-Choi-Lab" class="link-underline" style="color:var(--mono-accent);">github.com/UMN-Choi-Lab</a>/&lt;repo&gt;/issues<br/>
        // Tag with <span style="color:var(--mono-accent);">repro</span>.
      </p>
    </div>
  </div>

  <div class="mono-foot">
    <span>// end of module</span>
    <span class="accent">// back to editorial system ↓</span>
    <span>chois@umn:~/lab$ exit</span>
  </div>
</section>
</div>
