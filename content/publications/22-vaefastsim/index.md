---
title: "Particle-based fast jet simulation at the LHC with variational autoencoders"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
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

date: "2022-07-13T00:00:00Z"
doi: "10.1088/2632-2153/ac7c56"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "Machine Learning: Science and Technology"
publication_short: "Machine Learning: Science and Technology"

abstract: We study how to use deep variational autoencoders (VAEs) for a fast simulation of jets of particles at the Large Hadron Collider. We represent jets as a list of constituents, characterized by their momenta. Starting from a simulation of the jet before detector effects, we train a deep VAE to return the corresponding list of constituents after detection. Doing so, we bypass both the time-consuming detector simulation and the collision reconstruction steps of a traditional processing chain, speeding up significantly the events generation workflow. Through model optimization and hyperparameter tuning, we achieve state-of-the-art precision on the jet four-momentum, while providing an accurate description of the constituents momenta, and an inference time comparable to that of a rule-based fast simulation.

# Summary. An optional shortened abstract.
summary: ""

tags: ["ML", "Simulation"]

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2203.00520.pdf'
url_code: ''
url_arxiv: '2203.00520'
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
