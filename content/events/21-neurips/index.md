---
title: Particle Cloud Generation with Message Passing GANs
event_url: https://neurips.cc/virtual/2021/poster/28495
location: '[NeurIPS 21 (Virtual)](https://neurips.cc)'
summary: ''
abstract: In high energy physics (HEP), jets are collections of correlated particles produced ubiquitously in particle collisions such as those at the CERN Large Hadron Collider (LHC). Machine learning (ML)-based generative models, such as generative adversarial networks (GANs), have the potential to significantly accelerate LHC jet simulations. However, despite jets having a natural representation as a set of particles in momentum-space, a.k.a. a particle cloud, there exist no generative models applied to such a dataset. In this work, we introduce a new particle cloud dataset (JetNet), and apply to it existing point cloud GANs. Results are evaluated using (1) 1-Wasserstein distances between high- and low-level feature distributions, (2) a newly developed Fréchet ParticleNet Distance, and (3) the coverage and (4) minimum matching distance metrics. Existing GANs are found to be inadequate for physics applications, hence we develop a new message passing GAN (MPGAN), which outperforms existing point cloud GANs on virtually every metric and shows promise for use in HEP. We propose JetNet as a novel point-cloud-style dataset for the ML community to experiment with, and set MPGAN as a benchmark to improve upon for future generative models. Additionally, to facilitate research and improve accessibility and reproducibility in this area, we release the open-source JetNet Python package with interfaces for particle cloud datasets, implementations for evaluation and loss metrics, and more tools for ML in HEP development.
date: '2021-12-03T08:00:00Z'
authors: []
tags:
- ML
- Simulation
- HEP
- Equivariant and Physics-Informed ML
- Poster
featured: true
slug: neurips21
slides: null
projects:
- fast-sim
event_name: NeurIPS 21 Main Conference
event_start: '2021-12-03T08:00:00Z'
event_all_day: false
links:
- type: pdf
  url: https://github.com/rkansal47/MPGAN/blob/neurips21/NeurIPS21_Poster.pdf
- type: video
  url: https://neurips.cc/virtual/2021/poster/28495
---

