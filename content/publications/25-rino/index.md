---
title: "RINO: Renormalization Group Invariance with No Labels"

authors:
- Zichun Hao
- admin
- Abhijith Gandrakota
- Chang Sun
- Jennifer Ngadiuba
- Javier Duarte
- Maria Spiropulu

date: "2025-09-09T00:00:00Z"
doi: ""

publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

publication: "Machine Learning and the Physical Sciences Workshop @ NeurIPS 2025 (Spotlight)"
publication_short: "ML and the Physical Sciences Workshop @ NeurIPS (Spotlight)"

abstract: "A common challenge with supervised machine learning (ML) in high energy physics (HEP) is the reliance on simulations for labeled data, which can often mismodel the underlying collision or detector response. To help mitigate this problem of domain shift, we propose RINO (Renormalization Group Invariance with No Labels), a self-supervised learning approach that can instead pretrain models directly on collision data, learning embeddings invariant to renormalization group flow scales. In this work, we pretrain a transformer-based model on jets originating from quantum chromodynamic (QCD) interactions from the JetClass dataset, emulating real QCD-dominated experimental data, and then finetune on the JetNet dataset -- emulating simulations -- for the task of identifying jets originating from top quark decays. RINO demonstrates improved generalization from the JetNet training data to JetClass data compared to supervised training on JetNet from scratch, demonstrating the potential for RINO pretraining on real collision data followed by fine-tuning on small, high-quality MC datasets, to improve the robustness of ML models in HEP."

summary: "A novel physics-informed self-supervised pretraining strategy for foundation models in physics. SOTA results on transfer learning between simulations and real data."

tags: ["ML", "Equivariant and Physics-Informed ML"]

featured: true

url_pdf: 'https://ml4physicalsciences.github.io/2025/files/NeurIPS_ML4PS_2025_81.pdf'
url_code: ''
url_arxiv: '2509.07486'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

image:
  focal_point: "center"
  preview_only: false

projects: ['equivariant-networks']

---
