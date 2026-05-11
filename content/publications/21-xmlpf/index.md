---
title: "Explaining machine-learned particle-flow reconstruction"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
- Farouk Mokhtar
- admin
- Daniel Diaz
- Javier Duarte
- Joosep Pata
- Maurizio Pierini
- Jean-Roch Vlimant

date: "2021-12-01T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: Fourth Workshop on Machine Learning and the Physical Sciences @ NeurIPS 2021
publication_short: ML and the Physical Sciences Workshop @ NeurIPS 2021

abstract: The particle-flow (PF) algorithm is used in general-purpose particle detectors to reconstruct a comprehensive particle-level view of the collision by combining information from different subdetectors. A graph neural network (GNN) model, known as the machine-learned particle-flow (MLPF) algorithm, has been developed to substitute the rule-based PF algorithm. However, understanding the model's decision making is not straightforward, especially given the complexity of the set-to-set prediction task, dynamic graph building, and message-passing steps. In this paper, we adapt the layerwise-relevance propagation technique for GNNs and apply it to the MLPF algorithm to gauge the relevant nodes and features for its predictions. Through this process, we gain insight into the model's decision-making.

# Summary. An optional shortened abstract.
summary: "Developed a graph neural network model to reconstruct particle collisions and interpreted the results using explainable AI techniques."

tags: ["ML", "Simulation", "XAI"]

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2111.12840'
url_code: ''
url_arxiv: '2111.12840'
url_dataset: ''
url_poster: 'https://ml4physicalsciences.github.io/2021/files/NeurIPS_ML4PS_2021_120_poster.png'
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

projects: ['fast-sim', 'explainable-ai']

---
