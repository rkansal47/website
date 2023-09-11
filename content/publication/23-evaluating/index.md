---
title: "Evaluating generative models in high energy physics"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Anni Li
- Javier Duarte
- Nadezda Chernyavskaya
- Maurizio Pierini
- Breno Orzari
- Thiago Tomei

date: "2023-04-01T00:00:00Z"
doi: "10.1140/epjc/s10052-023-11633-5"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "Physical Review D"
publication_short: "Phys. Rev. D"

abstract: There has been a recent explosion in research into machine-learning-based generative modeling to tackle computational challenges for simulations in high energy physics (HEP). In order to use such alternative simulators in practice, we need well-defined metrics to compare different generative models and evaluate their discrepancy from the true distributions. We present the first systematic review and investigation into evaluation metrics and their sensitivity to failure modes of generative models, using the framework of two-sample goodness-of-fit testing, and their relevance and viability for HEP. Inspired by previous work in both physics and computer vision, we propose two new metrics, the Fréchet and kernel physics distances (FPD and KPD, respectively) and perform a variety of experiments measuring their performance on simple Gaussian-distributed and simulated high energy jet datasets. We find FPD, in particular, to be the most sensitive metric to all alternative jet distributions tested and recommend its adoption, along with the KPD and Wasserstein distances between individual feature distributions, for evaluating generative models in HEP. We finally demonstrate the efficacy of these proposed metrics in evaluating and comparing a novel attention-based generative adversarial particle transformer to the state-of-the-art message-passing generative adversarial network jet simulation model. The code for our proposed metrics is provided in the open source jetnet python library.

# Summary. An optional shortened abstract.
summary: "A systematic investigation of evaluation metrics for fast simulations, including two new ones we propose, the Fréchet and kernel physics distances, which we find to be the most sensitive. We also introduce the generative adversarial particle transformer (GAPT) model, which is significantly faster than MPGAN."

tags: ["ML", "Simulation"]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2211.10295.pdf'
url_code: 'https://github.com/rkansal47/MPGAN'
url_arxiv: '2211.10295'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  focal_point: "center"
  preview_only: false
  placement: 3


# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.

projects: ['fast-sim']

---
