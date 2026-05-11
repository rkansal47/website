---
title: Evaluating generative models in high energy physics
authors:
- admin
- Anni Li
- Javier Duarte
- Nadezda Chernyavskaya
- Maurizio Pierini
- Breno Orzari
- Thiago Tomei
date: '2023-04-01T00:00:00Z'
publishDate: '2017-01-01T00:00:00Z'
publication_types:
- article-journal
publication: Physical Review D
publication_short: Phys. Rev. D
abstract: There has been a recent explosion in research into machine-learning-based generative modeling to tackle computational challenges for simulations in high energy physics (HEP). In order to use such alternative simulators in practice, we need well-defined metrics to compare different generative models and evaluate their discrepancy from the true distributions. We present the first systematic review and investigation into evaluation metrics and their sensitivity to failure modes of generative models, using the framework of two-sample goodness-of-fit testing, and their relevance and viability for HEP. Inspired by previous work in both physics and computer vision, we propose two new metrics, the Fréchet and kernel physics distances (FPD and KPD, respectively) and perform a variety of experiments measuring their performance on simple Gaussian-distributed and simulated high energy jet datasets. We find FPD, in particular, to be the most sensitive metric to all alternative jet distributions tested and recommend its adoption, along with the KPD and Wasserstein distances between individual feature distributions, for evaluating generative models in HEP. We finally demonstrate the efficacy of these proposed metrics in evaluating and comparing a novel attention-based generative adversarial particle transformer to the state-of-the-art message-passing generative adversarial network jet simulation model. The code for our proposed metrics is provided in the open source jetnet python library.
summary: A systematic investigation of evaluation metrics for fast simulations, including two new ones we propose, the Fréchet and kernel physics distances, which we find to be the most sensitive. We also introduce the generative adversarial particle transformer (GAPT) model, which is significantly faster than MPGAN.
tags:
- ML
- Simulation
featured: true
image:
  focal_point: center
  preview_only: false
  placement: 3
projects:
- fast-sim
hugoblox:
  ids:
    doi: 10.1140/epjc/s10052-023-11633-5
    arxiv: '2211.10295'
links:
- type: custom
  name: arXiv
  url: https://arxiv.org/abs/2211.10295
- type: pdf
  url: https://arxiv.org/pdf/2211.10295.pdf
- type: code
  url: https://github.com/rkansal47/MPGAN
---

