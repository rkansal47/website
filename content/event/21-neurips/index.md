---
title: Particle Cloud Generation with Message Passing GANs

event: NeurIPS 21 Main Conference
event_url: https://neurips.cc/virtual/2021/poster/28495

talk_type: Poster

location: 'NeurIPS 21 (Virtual)'
location_link: https://neurips.cc

summary: ''
abstract: "In high energy physics (HEP), jets are collections of correlated particles produced ubiquitously in particle collisions such as those at the CERN Large Hadron Collider (LHC). Machine learning (ML)-based generative models, such as generative adversarial networks (GANs), have the potential to significantly accelerate LHC jet simulations. However, despite jets having a natural representation as a set of particles in momentum-space, a.k.a. a particle cloud, there exist no generative models applied to such a dataset. In this work, we introduce a new particle cloud dataset (JetNet), and apply to it existing point cloud GANs. Results are evaluated using (1) 1-Wasserstein distances between high- and low-level feature distributions, (2) a newly developed Fréchet ParticleNet Distance, and (3) the coverage and (4) minimum matching distance metrics. Existing GANs are found to be inadequate for physics applications, hence we develop a new message passing GAN (MPGAN), which outperforms existing point cloud GANs on virtually every metric and shows promise for use in HEP. We propose JetNet as a novel point-cloud-style dataset for the ML community to experiment with, and set MPGAN as a benchmark to improve upon for future generative models. Additionally, to facilitate research and improve accessibility and reproducibility in this area, we release the open-source JetNet Python package with interfaces for particle cloud datasets, implementations for evaluation and loss metrics, and more tools for ML in HEP development."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2021-12-03T08:00:00Z"
# <!-- date_end: "2030-06-01T15:00:00Z" -->
all_day: false

# Schedule page publish date (NOT talk date).
# publishDate: "2017-01-01T00:00:00Z"

authors: []
tags: ["ML", "Simulation", "HEP", "Equivariant and Physics-Informed ML"]

# Is this a featured talk? (true/false)
featured: true

links:
url_code: ""
url_pdf: "https://github.com/rkansal47/MPGAN/blob/neurips21/NeurIPS21_Poster.pdf"
url_slides: ""
url_video: "https://neurips.cc/virtual/2021/poster/28495"

slug: neurips21

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides:

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects:
- fast-sim
---
