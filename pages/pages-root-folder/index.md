---
layout: editorial
title: Home
editorial_page: Home
permalink: /index.html
homepage: true
---

<!-- HERO -->
<section class="hero">
  <div>
    <p class="kicker kicker-mark">Lead · Who &amp; why</p>
    <h1>Turning <em>messy city data</em> into operational insight.</h1>
    <p class="lede">I'm an Assistant Professor in Civil, Environmental, and Geo-Engineering at the University of Minnesota, Twin Cities. My lab works on urban mobility data analytics, spatiotemporal modeling, and deep generative AI — in service of more sustainable, efficient transportation systems.</p>
    <div class="tag-row">
      <a href="{{ site.baseurl }}/research/" class="naked">Generative intelligence</a>
      <a href="{{ site.baseurl }}/research/" class="naked">Vision-Language-Action models</a>
      <a href="{{ site.baseurl }}/research/" class="naked">LLM-powered traffic management</a>
      <a href="{{ site.baseurl }}/research/" class="naked">Spatiotemporal forecasting</a>
      <a href="{{ site.baseurl }}/research/" class="naked">Deep learning for transportation</a>
    </div>
    <div class="quick-links">
      <a href="{{ site.baseurl }}/about/" class="link-underline">About →</a>
      <a href="{{ site.baseurl }}/publications/" class="link-underline">Publications →</a>
      <a href="{{ site.baseurl }}/datacode/" class="link-underline">Data &amp; Code →</a>
    </div>
  </div>
  <div>
    <div class="placeholder" style="height:300px;">
      <span class="label">[ headshot — drop image ]</span>
    </div>
    <div class="hero-side">
      <div>Office · Civil Eng. Bldg. 142</div>
      <div>500 Pillsbury Drive SE · Minneapolis</div>
      <div class="links">
        <a href="https://scholar.google.com/citations?user=tyLWFk4AAAAJ" class="link-underline">Scholar ↗</a>
        <a href="https://github.com/UMN-Choi-Lab" class="link-underline">GitHub ↗</a>
        <a class="link-underline">CV (PDF) ↓</a>
      </div>
    </div>
  </div>
</section>

<!-- FEATURED PAPERS -->
<section class="section">
  <div class="section-head">
    <div>
      <p class="kicker kicker-mark">Section I · Featured</p>
      <h2>Three papers, this season.</h2>
    </div>
    <a href="{{ site.baseurl }}/publications/" class="link-underline more-link">All publications →</a>
  </div>
  <div class="featured-grid">
    <article class="featured-card">
      <div class="num">01</div>
      <div class="venue">2025 · <em>Transportation Research Part C</em></div>
      <h3>A Gentle Introduction &amp; Tutorial on Deep Generative Models in Transportation Research</h3>
      <div class="authors"><strong>Choi, S.</strong>, Jin, Z., Ham, S. W., Kim, J., Sun, L.</div>
      <div class="row-links">
        <a href="https://choi-seongjin.github.io/publist/gentle2025choi.pdf" class="link-underline">PDF</a>
        <a href="https://doi.org/10.1016/j.trc.2025.105145" class="link-underline">DOI ↗</a>
      </div>
    </article>
    <article class="featured-card">
      <div class="num">02</div>
      <div class="venue">2025 · <em>NeurIPS · Datasets &amp; Benchmarks</em></div>
      <h3>BO4Mob: Bayesian Optimization Benchmarks for High-Dimensional Urban Mobility</h3>
      <div class="authors">Ryu, S., Kwon, D., <strong>Choi, S.</strong>, Deshwal, A., Kang, S., Osorio, C.</div>
      <div class="row-links">
        <a class="link-underline">PDF</a>
        <a class="link-underline">Code ↗</a>
      </div>
    </article>
    <article class="featured-card">
      <div class="num">03</div>
      <div class="venue">2025 · <em>Transportation Science</em></div>
      <h3>Scalable Dynamic Mixture Model with Full Covariance for Probabilistic Traffic Forecasting</h3>
      <div class="authors"><strong>Choi, S.</strong>, Saunier, N., Zheng, V. Z., Trépanier, M., Sun, L.</div>
      <div class="row-links">
        <a href="https://choi-seongjin.github.io/publist/scalable2025choi.pdf" class="link-underline">PDF</a>
        <a href="https://doi.org/10.1287/trsc.2024.0547" class="link-underline">DOI ↗</a>
      </div>
    </article>
  </div>
</section>

<!-- NEWS -->
<section class="section soft">
  <div class="section-head">
    <div>
      <p class="kicker kicker-mark">Section II · Recent activity</p>
      <h2>News &amp; notes.</h2>
    </div>
    <a href="{{ site.baseurl }}/news/" class="link-underline more-link">All news →</a>
  </div>
  <div class="news-grid">
    {% assign recent = site.posts | slice: 0, 3 %}
    {% for post in recent %}
    <article class="news-card">
      <div class="meta">{{ post.date | date: "%Y·%m·%d" }} · <span class="tag">{% if post.tag %}{{ post.tag }}{% else %}News{% endif %}</span></div>
      <h3>{{ post.title | remove: "[" | remove: "]" | replace: "260112 ", "" | replace: "250307 ", "" | replace: "250420 ", "" }}</h3>
      <p>{{ post.teaser | strip_html | truncate: 220 }}</p>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read">Read →</a>
    </article>
    {% endfor %}
  </div>
</section>

<!-- THE SEAM — Data & Code preview module in BRUT -->
<section class="mono-module mono-preview">
  <div class="terminal-bar">
    <span>// system:brut · module = data_and_code preview</span>
    <span class="progress">▮▮▮▮▮▮▮▮▯▯ &nbsp; preview</span>
    <span>$ ls -la</span>
  </div>
  <div class="mono-hero">
    <div>
      <p class="kicker kicker-mark">Lab notebook · preview</p>
      <h2 class="big">REPOS &amp;<br/><span class="accent">DATASETS.</span></h2>
      <p>// Every featured paper ships with a repo and, where licensable, a dataset.<br/>
         // Stars + last-commit cached at build time — no live API calls.</p>
    </div>
    <div class="side-card" style="text-align:right;">
      <div>Public repos · <span style="color:var(--mono-fg);">tbd</span></div>
      <div>Archived datasets · <span style="color:var(--mono-fg);">tbd</span></div>
      <div class="sep">
        <a href="{{ site.baseurl }}/datacode/" class="link-underline">All repos &amp; data →</a>
      </div>
    </div>
  </div>
  <div style="padding:0 var(--pad-x) 44px;">
    <div class="repos-table">
      <div class="row head">
        <span>№</span><span>Repository</span><span>Description</span><span>Lang</span><span>★</span><span>Updated</span>
      </div>
      <a href="{{ site.baseurl }}/datacode/" class="row repo-row naked" data-tags="GenAI">
        <span class="num">01</span>
        <span class="repo">~/UMN-Choi-Lab/[ pending ]</span>
        <span class="desc">A handle for the lab's public repositories — list to be populated as papers are released.</span>
        <span>Python</span>
        <span>★ —</span>
        <span class="upd">—</span>
      </a>
      <div style="padding:18px 0;color:var(--mono-sub);font-family:var(--mfont);font-size:12px;">
        // Repos list pending — open Data &amp; Code for the full module.
      </div>
    </div>
  </div>
</section>

<!-- RESEARCH AREAS -->
<section class="section" style="border-top:4px solid var(--accent);">
  <div class="section-head">
    <div>
      <p class="kicker kicker-mark">Section IV · Areas</p>
      <h2>Three lines of work.</h2>
    </div>
  </div>
  <div class="areas-grid" style="grid-template-columns: repeat(3, 1fr);">
    <a class="area-card naked" href="{{ site.baseurl }}/research/">
      <div class="n">N° 01</div>
      <div class="title-area">Generative Intelligence for Transportation Modeling</div>
      <div class="more">Read more →</div>
    </a>
    <a class="area-card naked" href="{{ site.baseurl }}/research/">
      <div class="n">N° 02</div>
      <div class="title-area">Vision-Language-Action Models for Autonomous Driving</div>
      <div class="more">Read more →</div>
    </a>
    <a class="area-card naked" href="{{ site.baseurl }}/research/">
      <div class="n">N° 03</div>
      <div class="title-area">TMC-Agent · LLM-Powered Traffic Management</div>
      <div class="more">Read more →</div>
    </a>
  </div>
</section>

<!-- RECRUITING -->
<section class="recruit-block" id="recruiting">
  <div>
    <p class="kicker">◆ Classified · Fall 2026</p>
    <h2>Wanted: curious PhDs.</h2>
    <p>Looking for PhD students (and a postdoc) excited about machine learning for urban mobility. Please email <span style="border-bottom:1px solid currentColor;">chois@umn.edu</span> with CV, research statement, and transcript. Subject: "Prospective PhD student [Your name]".</p>
  </div>
  <div class="card">
    <div class="head">Reply by email</div>
    <div class="email">chois@umn.edu</div>
    <div class="sep">Subject: "Prospective PhD student [Your name]". Attach: CV, research statement, transcript.</div>
  </div>
</section>
