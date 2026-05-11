---
title: Particle-based fast jet simulation at the LHC with variational autoencoders
authors:
- Mary Touranakou
- Nadezda Chernyavskaya
- Javier Duarte
- Dimitrios Gunopulos
- admin
- Breno Orzari
- Maurizio Pierini
- Thiago Tomei
- Jean-Roch Vlimant
date: '2022-07-13T00:00:00Z'
publishDate: '2017-01-01T00:00:00Z'
publication_types:
- article-journal
publication: 'Machine Learning: Science and Technology'
publication_short: 'Machine Learning: Science and Technology'
abstract: We study how to use deep variational autoencoders (VAEs) for a fast simulation of jets of particles at the Large Hadron Collider. We represent jets as a list of constituents, characterized by their momenta. Starting from a simulation of the jet before detector effects, we train a deep VAE to return the corresponding list of constituents after detection. Doing so, we bypass both the time-consuming detector simulation and the collision reconstruction steps of a traditional processing chain, speeding up significantly the events generation workflow. Through model optimization and hyperparameter tuning, we achieve state-of-the-art precision on the jet four-momentum, while providing an accurate description of the constituents momenta, and an inference time comparable to that of a rule-based fast simulation.
summary: ''
tags:
- ML
- Simulation
featured: false
image:
  focal_point: center
  preview_only: false
projects:
- fast-sim
hugoblox:
  ids:
    doi: 10.1088/2632-2153/ac7c56
    arxiv: '2203.00520'
links:
- type: custom
  name: arXiv
  url: https://arxiv.org/abs/2203.00520
- type: pdf
  url: https://arxiv.org/pdf/2203.00520.pdf
---

