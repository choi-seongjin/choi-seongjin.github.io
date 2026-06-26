---
layout: quiet
title: Home
permalink: /
---

<!-- HERO -->
<section class="q-hero">
  <p class="q-eyebrow">University of Minnesota · Choi Lab</p>
  <h1>AI that turns <em>messy city data</em> into operational insight.</h1>
  <p class="q-lede">We're the Choi Lab in Civil, Environmental, and Geo-Engineering at the University of Minnesota, Twin Cities — building AI for urban mobility with deep generative models, vision-language-action models, and LLM agents, in service of more sustainable, efficient transportation systems.</p>
  <div class="q-btn-row">
    <a class="q-btn primary" href="{{ site.baseurl }}/research/">Read the research →</a>
    <a class="q-btn secondary" href="{{ site.baseurl }}/PI/#recruiting">Recruiting · PhD &amp; Postdoc · Fall 2027</a>
  </div>
</section>

<!-- RESEARCH AREAS -->
<section class="q-section">
  <div class="q-sec-head">
    <h2 class="q-h2">Research areas</h2>
    <a class="q-more" href="{{ site.baseurl }}/research/">All projects →</a>
  </div>
  <div class="q-areas">
    <a class="q-area" href="{{ site.baseurl }}/research/">
      <div class="q-area-chip">01</div>
      <h3>Generative Intelligence for Transportation Modeling</h3>
      <p>Diffusion, normalizing flows, GANs, and probabilistic mixtures for traffic state estimation, trajectory generation, and probabilistic forecasting — beyond deterministic point estimates.</p>
    </a>
    <a class="q-area" href="{{ site.baseurl }}/research/">
      <div class="q-area-chip">02</div>
      <h3>AI-Powered Connected and Automated Driving</h3>
      <p>Multimodal foundation and Vision-Language-Action models, plus deep RL for cooperative driving and vehicle control — extending to traffic-surveillance tasks like vehicle identification and monitoring.</p>
    </a>
    <a class="q-area" href="{{ site.baseurl }}/research/">
      <div class="q-area-chip">03</div>
      <h3>TMC-Agent · LLM-Powered Traffic Management</h3>
      <p>LLM-powered agents that augment Traffic Management Center operators — interpreting network data, enabling natural-language interaction, and supporting real-time decisions.</p>
    </a>
  </div>
</section>

<!-- RECENT PUBLICATIONS (3 blocks + list, 4-up) -->
<section class="q-section panel">
  <div class="q-sec-head">
    <h2 class="q-h2">Recent publications</h2>
    <a class="q-more" href="{{ site.baseurl }}/publications/">All publications →</a>
  </div>
  <div class="q-recent">
    <a class="q-recent-block" href="https://doi.org/10.1109/TITS.2026.3651399">
      <div class="q-fig"><img src="{{ site.baseurl }}/assets/images/pub/cho2026toward.png" alt="UAM route feasibility — probabilistic aircraft trajectory prediction over Seoul terminal airspace" /></div>
      <div class="venue">IEEE Trans. Intelligent Transportation Systems · 2026</div>
      <h3>Toward Safe Integration of UAM in Terminal Airspace: Route Feasibility via Probabilistic Aircraft Trajectory Prediction</h3>
    </a>
    <a class="q-recent-block" href="https://arxiv.org/abs/2512.06183">
      <div class="q-fig"><img src="{{ site.baseurl }}/assets/images/pub/liu2026pma.png" alt="PMA-Diffusion — space-time traffic state estimation from sparse observations" /></div>
      <div class="venue">Transportation Research Part C · in press</div>
      <h3>PMA-Diffusion: A Physics-guided Mask-aware Diffusion Framework for Traffic State Estimation from Sparse Observations</h3>
    </a>
    <a class="q-recent-block" href="https://arxiv.org/abs/2510.18824">
      <div class="q-fig"><img src="{{ site.baseurl }}/assets/images/pub/ryu2025bo4mob.png" alt="BO4Mob — origin-destination demand estimation benchmark network with sensors" /></div>
      <div class="venue">NeurIPS Datasets &amp; Benchmarks · 2025</div>
      <h3>BO4Mob: Bayesian Optimization Benchmarks for High-Dimensional Urban Mobility</h3>
    </a>
    <div class="q-recent-list">
      <div class="head">More recent</div>
      <ul>
        <li><a href="{{ site.baseurl }}/publications/#choi2025gentle">A Gentle Introduction &amp; Tutorial on Deep Generative Models<span>Transportation Research Part C · 2025</span></a></li>
        <li><a href="{{ site.baseurl }}/publications/#kim2026nextsim">NextSim: Multi-Level Traffic Simulation for Urban Networks<span>IEEE Trans. ITS · 2026</span></a></li>
        <li><a href="{{ site.baseurl }}/publications/#choi2025scalable">Scalable Dynamic Mixture Model for Probabilistic Forecasting<span>Transportation Science · 2025</span></a></li>
        <li><a href="{{ site.baseurl }}/publications/#jiang2025survey">A Survey on Vision-Language-Action Models for Autonomous Driving<span>ICCV Workshops · 2025</span></a></li>
      </ul>
    </div>
  </div>
</section>

<!-- HIGHLIGHTED PROJECTS (real repos) -->
<section class="q-section">
  <div class="q-sec-head">
    <h2 class="q-h2">Highlighted projects</h2>
    <a class="q-more" href="{{ site.baseurl }}/datacode/">All repos &amp; data →</a>
  </div>
  <div class="q-projects">
    <a class="q-proj" href="{{ site.baseurl }}/transport-atlas/">
      <span class="tag">Atlas · Bibliometrics</span><h3>Transport Atlas</h3>
      <p>Interactive explorer of the transportation research literature — coauthorship network, author trajectories, topic space, venues, and a reviewer finder.</p>
      <span class="meta">Live · Interactive</span>
    </a>
    <a class="q-proj" href="https://github.com/benchoi93/TrajGAIL">
      <span class="tag">GenAI · Trajectories</span><h3>TrajGAIL</h3>
      <p>Urban vehicle trajectory generation via generative adversarial imitation learning (TR-C 2021).</p>
      <span class="meta">★ 68 · Python</span>
    </a>
    <a class="q-proj" href="https://github.com/UMN-Choi-Lab/BO4Mob">
      <span class="tag">Benchmark · OD</span><h3>BO4Mob</h3>
      <p>Bayesian optimization benchmarks for high-dimensional urban mobility (NeurIPS 2025 D&amp;B).</p>
      <span class="meta">★ 18 · Python</span>
    </a>
    <a class="q-proj" href="https://github.com/UMN-Choi-Lab/DGMinTransportation">
      <span class="tag">Survey</span><h3>DGMinTransportation</h3>
      <p>Companion code &amp; notebooks for the TR-C 2025 deep generative models survey.</p>
      <span class="meta">★ 9 · Jupyter</span>
    </a>
    <a class="q-proj" href="https://github.com/UMN-Choi-Lab/TrajFlow">
      <span class="tag">GenAI</span><h3>TrajFlow</h3>
      <p>Normalizing-flow framework for occupancy density estimation from trajectories.</p>
      <span class="meta">★ 3 · Python</span>
    </a>
    <a class="q-proj" href="https://github.com/UMN-Choi-Lab/TrafficNetQA">
      <span class="tag">LLM</span><h3>TrafficNetQA</h3>
      <p>QA benchmark for evaluating LLM performance on traffic network files (SIGSPATIAL 2025).</p>
      <span class="meta">★ 1 · Python</span>
    </a>
    <a class="q-proj" href="https://github.com/UMN-Choi-Lab/camera2detector">
      <span class="tag">Vision · Sensing</span><h3>camera2detector</h3>
      <p>Real-time camera validation of MnDOT highway detectors using YOLO computer vision.</p>
      <span class="meta">★ 1 · Python</span>
    </a>
    <a class="q-proj" href="https://github.com/UMN-Choi-Lab/HighwayVLM">
      <span class="tag">VLA · Safety</span><h3>HighwayVLM</h3>
      <p>Open-source highway-safety analysis with vision-language models.</p>
      <span class="meta">★ 1 · Python</span>
    </a>
    <a class="q-proj" href="https://github.com/UMN-Choi-Lab/ODS_PLD">
      <span class="tag">OD</span><h3>ODS_PLD</h3>
      <p>Analytical OD estimation via NNLS and Projected Langevin Dynamics, validated under SUMO.</p>
      <span class="meta">★ 0 · Python</span>
    </a>
    <a class="q-proj" href="https://github.com/UMN-Choi-Lab/SynPopPred">
      <span class="tag">LLM</span><h3>SynPopPred</h3>
      <p>LLM-based synthetic population generation — IPF, CTGAN, DistilGPT-2, and Llama 3.1 8B.</p>
      <span class="meta">★ 0 · Python</span>
    </a>
  </div>
</section>

<!-- THE TEAM -->
<section class="q-section panel">
  <div class="q-sec-head">
    <h2 class="q-h2">The team</h2>
    <a class="q-more" href="{{ site.baseurl }}/team/">Full team &amp; alumni →</a>
  </div>
  <div class="q-team">
    <div class="q-person">
      <div class="q-fig"><img src="{{ site.baseurl }}/images/profile_sjchoi_2026.jpg" alt="Seongjin Choi" /></div>
      <h3><a href="{{ site.baseurl }}/PI/" style="color:var(--accent);">Seongjin Choi</a></h3>
      <div class="role">Principal Investigator · Assistant Professor</div>
      <div class="sub">AI for urban mobility · generative models · VLA · LLM agents</div>
    </div>
    <div class="q-person">
      <div class="q-fig"><img src="{{ site.baseurl }}/images/profile_guoliang.jpg" alt="Guoliang Feng" /></div>
      <h3>Guoliang Feng</h3>
      <div class="role">Postdoctoral Researcher</div>
      <div class="sub">AI in traffic operation · agentic simulation</div>
    </div>
    <div class="q-person">
      <div class="q-fig"><img src="{{ site.baseurl }}/images/profile_lindong.jpg" alt="Lindong Liu" /></div>
      <h3>Lindong Liu</h3>
      <div class="role">PhD · CEGE · 2024 –</div>
      <div class="sub">Inverse problems · traffic state estimation</div>
    </div>
    <div class="q-person">
      <div class="q-fig"></div>
      <h3>Christopher Cheong</h3>
      <div class="role">PhD · CEGE · 2025 –</div>
      <div class="sub">Traffic forecasting · spatiotemporal nets</div>
    </div>
    <div class="q-person">
      <div class="q-fig"></div>
      <h3><a href="https://pouya-parsa.github.io/" target="_blank" rel="noopener" style="color:var(--accent);">Pouya Parsa</a></h3>
      <div class="role">PhD · CEGE · 2026 –</div>
      <div class="sub">Scalable VLA models for autonomous driving</div>
    </div>
    <div class="q-person">
      <div class="q-fig"></div>
      <h3>Rammesh Adhav Saravanan</h3>
      <div class="role">MS · MnRI · 2024 –</div>
      <div class="sub">Cooperative VLA models for autonomous driving</div>
    </div>
  </div>
</section>
