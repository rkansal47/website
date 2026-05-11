---
title: Sparse Data Generation for Particle-Based Simulation of Hadronic Jets in the LHC
authors:
- Breno Orzari
- Thiago Tomei
- Maurizio Pierini
- Mary Touranakou
- Javier Duarte
- admin
- Jean-Roch Vlimant
- Dimitrios Gunopulos
date: '2021-09-21T00:00:00Z'
publishDate: '2017-01-01T00:00:00Z'
publication_types:
- article-journal
publication: LatinX in AI Research Workshop @ ICML 2021
publication_short: LatinX in AI Research Workshop @ ICML 2021
abstract: We develop a generative neural network for the generation of sparse data in particle physics using a permutation-invariant and physics-informed loss function. The input dataset used in this study consists of the particle constituents of hadronic jets due to its sparsity and the possibility of evaluating the network's ability to accurately describe the particles and jets properties. A variational autoencoder composed of convolutional layers in the encoder and decoder is used as the generator. The loss function consists of a reconstruction error term and the Kullback-Leibler divergence between the output of the encoder and the latent vector variables. The permutation-invariant loss on the particles' properties is combined with two mean-squared error terms that measure the difference between input and output jets mass and transverse momentum, which improves the network's generation capability as it imposes physics constraints, allowing the model to learn the kinematics of the jets.
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
    arxiv: '2109.15197'
links:
- type: custom
  name: arXiv
  url: https://arxiv.org/abs/2109.15197
- type: pdf
  url: https://arxiv.org/pdf/2109.15197.pdf
---

