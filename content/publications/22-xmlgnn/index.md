---
title: Do graph neural networks learn traditional jet substructure?
authors:
- Farouk Mokhtar
- admin
- Javier Duarte
date: '2022-12-09T00:00:00Z'
publishDate: '2017-01-01T00:00:00Z'
publication_types:
- paper-conference
publication: Fifth Workshop on Machine Learning and the Physical Sciences @ NeurIPS 2022
publication_short: ML and the Physical Sciences Workshop @ NeurIPS 2022
abstract: At the CERN LHC, the task of jet tagging, whose goal is to infer the origin of a jet given a set of final-state particles, is dominated by machine learning methods. Graph neural networks have been used to address this task by treating jets as point clouds with underlying, learnable, edge connections between the particles inside. We explore the decision-making process for one such state-of-the-art network, ParticleNet, by looking for relevant edge connections identified using the layerwise-relevance propagation technique. As the model is trained, we observe changes in the distribution of relevant edges connecting different intermediate clusters of particles, known as subjets. The resulting distribution of subjet connections is different for signal jets originating from top quarks, whose subjets typically correspond to its three decay products, and background jets originating from lighter quarks and gluons. This behavior indicates that the model is using traditional jet substructure observables, such as the number of prongs -- energetic particle clusters -- within a jet, when identifying jets.
summary: ''
tags:
- ML
- XAI
featured: false
image:
  focal_point: center
  preview_only: false
projects:
- explainable-ai
hugoblox:
  ids:
    arxiv: '2211.09912'
links:
- type: custom
  name: arXiv
  url: https://arxiv.org/abs/2211.09912
- type: pdf
  url: https://arxiv.org/pdf/2211.09912
- type: poster
  url: https://neurips.cc/media/PosterPDFs/NeurIPS%202022/56928.png
---

