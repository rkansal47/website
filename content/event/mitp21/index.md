---
title: Particle Cloud Generation with Message Passing GANs

event: MITP Machine Learning for Particle Physics Workshop
event_url: https://indico.mitp.uni-mainz.de/event/199/overview

location: Mainz Institute for Theoretical Physics (Invited Talk, Virtual)
location_link: https://www.mitp.uni-mainz.de

summary: ''
abstract: "In high energy physics (HEP), jets are collections of correlated particles produced ubiquitously in particle collisions such as those at the CERN Large Hadron Collider (LHC). Machine-learning-based generative models, such as generative adversarial networks (GANs), have the potential to significantly accelerate LHC jet simulations. However, despite jets having a natural representation as a set of particles in momentum-space, a.k.a. a particle cloud, to our knowledge there exist no generative models applied to such a dataset. We introduce a new particle cloud dataset (JetNet), and, due to similarities between particle and point clouds, apply to it existing point cloud GANs. Results are evaluated using (1) the 1-Wasserstein distance between high- and low-level feature distributions, (2) a newly developed Fréchet ParticleNet Distance, and (3) the coverage and (4) minimum matching distance metrics. Existing GANs are found to be inadequate for physics applications, hence we develop a new message passing GAN (MPGAN), which outperforms existing point cloud GANs on virtually every metric and shows promise for use in HEP. We propose JetNet as a novel point-cloud-style dataset for the machine learning community to experiment with, and set MPGAN as a benchmark to improve upon for future generative models."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2021-06-23T08:00:00Z"
# <!-- date_end: "2030-06-01T15:00:00Z" -->
all_day: false

# Schedule page publish date (NOT talk date).
# publishDate: "2017-01-01T00:00:00Z"

authors: []
tags: []

# Is this a featured talk? (true/false)
featured: true

links:
url_code: ""
url_pdf: ""
url_slides: "https://www.icloud.com/keynote/0NOJMOE4ex1eXjZ3BwxH_Zm7w#MITP_MLPP_Workshop_23/06/21"
url_video: ""

slug: mitp21

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
- graph-gan
---
