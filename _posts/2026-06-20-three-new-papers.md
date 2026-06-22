---
layout: page-fullwidth
title: "Three new papers: PMA-Diffusion, Weaver, and TrajFlow"
meta_title: ""
subheadline: "Publications"
teaser: "A great stretch for the lab: PMA-Diffusion is published in Transportation Research Part C, while Weaver (also TR Part C) and TrajFlow (Artificial Intelligence for Transportation) have been accepted and are now in press."
permalink: "/news/260620"
header: no
readmore: true
---

I'm excited to share three new papers from the lab, all on generative and deep-learning methods for traffic modeling.

**PMA-Diffusion: A Physics-guided Mask-aware Diffusion Framework for Traffic State Estimation from Sparse Observations** has been published in *Transportation Research Part C: Emerging Technologies* (Volume 190, Article 105801). Led by **Lindong Liu**, together with **Zhixiong Jin**, this work reformulates sparse traffic state estimation as a Bayesian inverse problem. Instead of requiring fully observed training data, PMA-Diffusion learns a mask-aware diffusion prior directly from incomplete speed fields and applies weak traffic-physics guidance only at inference through an adaptive anisotropic smoothing projector. On the I-24 MOTION dataset it reconstructs complete highway speed fields even under severe sparsity—outperforming representative baselines at as little as 5% visibility.

- 📄 [DOI: 10.1016/j.trc.2026.105801 ↗](https://doi.org/10.1016/j.trc.2026.105801)

**Weaver: Kronecker Product Approximations of Spatiotemporal Attention for Traffic Network Forecasting**, by **Christopher Cheong**, **Gary Davis**, and me, has been accepted and is in press at *Transportation Research Part C: Emerging Technologies*. Weaver uses the mixed Kronecker matrix–vector identity to approximate spatiotemporal attention efficiently, factorizing spatial and temporal structure to scale attention-based forecasting to large traffic networks.

- 📄 [arXiv:2511.08888 ↗](https://arxiv.org/abs/2511.08888)

**TrajFlow: A Generative Framework for Occupancy Density Estimation Using Normalizing Flows**, by **Mitch Kosieradzki** and me, has been accepted and is in press at *Artificial Intelligence for Transportation*. TrajFlow casts occupancy density estimation as a generative modeling problem, using normalizing flows to learn flexible, tractable densities over future trajectory occupancy.

- 📄 [arXiv:2501.14266 ↗](https://arxiv.org/abs/2501.14266)

Congratulations to Lindong, Chris, Mitch, and all of our collaborators on these milestones! 🎉
