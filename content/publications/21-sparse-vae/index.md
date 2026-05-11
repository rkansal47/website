---
title: "Sparse Data Generation for Particle-Based Simulation of Hadronic Jets in the LHC"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
- Breno Orzari
- Thiago Tomei
- Maurizio Pierini
- Mary Touranakou
- Javier Duarte
- admin
- Jean-Roch Vlimant
- Dimitrios Gunopulos

date: "2021-09-21T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "LatinX in AI Research Workshop @ ICML 2021"
publication_short: "LatinX in AI Research Workshop @ ICML 2021"

abstract: We develop a generative neural network for the generation of sparse data in particle physics using a permutation-invariant and physics-informed loss function. The input dataset used in this study consists of the particle constituents of hadronic jets due to its sparsity and the possibility of evaluating the network's ability to accurately describe the particles and jets properties. A variational autoencoder composed of convolutional layers in the encoder and decoder is used as the generator. The loss function consists of a reconstruction error term and the Kullback-Leibler divergence between the output of the encoder and the latent vector variables. The permutation-invariant loss on the particles' properties is combined with two mean-squared error terms that measure the difference between input and output jets mass and transverse momentum, which improves the network's generation capability as it imposes physics constraints, allowing the model to learn the kinematics of the jets.

# Summary. An optional shortened abstract.
summary: ""

tags: ["ML", "Simulation"]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2109.15197.pdf'
url_code: ''
url_arxiv: '2109.15197'
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


# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.

projects: ['fast-sim']

---
