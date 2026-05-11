---
title: Particle Cloud Generation with Message Passing Generative Adversarial Networks
authors:
- admin
- Javier Duarte
- Hao Su
- Breno Orzari
- Thiago Tomei
- Maurizio Pierini
- Mary Touranakou
- Jean-Roch Vlimant
- Dimitrios Gunopulos
date: '2021-12-03T00:00:00Z'
publishDate: '2017-01-01T00:00:00Z'
publication_types:
- paper-conference
publication: Advances in Neural Information Processing Systems (NeurIPS 2021)
publication_short: NeurIPS 2021
abstract: In high energy physics (HEP), jets are collections of correlated particles produced ubiquitously in particle collisions such as those at the CERN Large Hadron Collider (LHC). Machine learning (ML)-based generative models, such as generative adversarial networks (GANs), have the potential to significantly accelerate LHC jet simulations. However, despite jets having a natural representation as a set of particles in momentum-space, a.k.a. a particle cloud, there exist no generative models applied to such a dataset. In this work, we introduce a new particle cloud dataset (JetNet), and apply to it existing point cloud GANs. Results are evaluated using (1) 1-Wasserstein distances between high- and low-level feature distributions, (2) a newly developed Fréchet ParticleNet Distance, and (3) the coverage and (4) minimum matching distance metrics. Existing GANs are found to be inadequate for physics applications, hence we develop a new message passing GAN (MPGAN), which outperforms existing point cloud GANs on virtually every metric and shows promise for use in HEP. We propose JetNet as a novel point-cloud-style dataset for the ML community to experiment with, and set MPGAN as a benchmark to improve upon for future generative models. Additionally, to facilitate research and improve accessibility and reproducibility in this area, we release the open-source JetNet Python package with interfaces for particle cloud datasets, implementations for evaluation and loss metrics, and more tools for ML in HEP development.
summary: Introduces the message-passing generative adversarial (MPGAN) model and JetNet dataset. We found the physics-informed MPGAN model outperformed all existing point-cloud GANs in simulating high momentum jets.
tags:
- ML
- Simulation
- Equivariant and Physics-Informed ML
- Datasets
featured: true
image:
  focal_point: center
  preview_only: false
projects:
- fast-sim
hugoblox:
  ids:
    arxiv: '2106.11535'
links:
- type: custom
  name: arXiv
  url: https://arxiv.org/abs/2106.11535
- type: pdf
  url: https://arxiv.org/pdf/2106.11535.pdf
- type: code
  url: https://github.com/rkansal47/MPGAN
- type: dataset
  url: https://zenodo.org/record/4834876#.YNlNgy1w2J8
---

