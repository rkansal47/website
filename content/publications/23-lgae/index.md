---
title: Lorentz group equivariant autoencoders
authors:
- Zichun Hao
- admin
- Javier Duarte
- Nadezda Chernyavskaya
date: '2023-06-09T00:00:00Z'
publishDate: '2017-01-01T00:00:00Z'
publication_types:
- article-journal
publication: The European Physical Journal C
publication_short: Eur. Phys. J. C
abstract: There has been significant work recently in developing machine learning (ML) models in high energy physics (HEP) for tasks such as classification, simulation, and anomaly detection. Often these models are adapted from those designed for datasets in computer vision or natural language processing, which lack inductive biases suited to HEP data, such as equivariance to its inherent symmetries. Such biases have been shown to make models more performant and interpretable, and reduce the amount of training data needed. To that end, we develop the Lorentz group autoencoder (LGAE), an autoencoder model equivariant with respect to the proper, orthochronous Lorentz group SO+(3,1), with a latent space living in the representations of the group. We present our architecture and several experimental results on jets at the LHC and find it outperforms graph and convolutional neural network baseline models on several compression, reconstruction, and anomaly detection metrics. We also demonstrate the advantage of such an equivariant model in analyzing the latent space of the autoencoder, which can improve the explainability of potential anomalies discovered by such ML models.
summary: Developed an auto-encoder model equivariant to Lorentz transformations of the input. We find it outperforms graph and convolutional neural networks on jet reconstruction and anomaly detection tasks.
tags:
- ML
- Equivariant and Physics-Informed ML
- Anomaly Detection
featured: true
image:
  focal_point: center
  preview_only: false
projects:
- equivariant-networks
- anomaly-detection
hugoblox:
  ids:
    doi: 10.1140/epjc/s10052-023-11633-5
    arxiv: '2212.07347'
links:
- type: custom
  name: arXiv
  url: https://arxiv.org/abs/2212.07347
- type: pdf
  url: https://arxiv.org/pdf/2212.07347.pdf
- type: code
  url: https://github.com/zichunhao/lgn-autoencoder
---

