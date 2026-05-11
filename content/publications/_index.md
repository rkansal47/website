---
title: Publications
cms_exclude: true
date: 2022-10-24
type: landing

sections:
  - block: portfolio
    id: featured
    content:
      title: Publications
      filters:
        folders:
          - publications
        featured_only: false
      archive:
        enable: false
      default_button_index: 0
      buttons:
        - name: All
          tag: '*'
        - name: "ML"
          tag: "ML"
        - name: "Higgs"
          tag: "Higgs"
        - name: "CMS"
          tag: "CMS"
        - name: "Simulation"
          tag: "Simulation"
        - name: "Anomaly Detection"
          tag: "Anomaly Detection"
        - name: "Equivariant / Physics-Informed ML"
          tag: "Equivariant and Physics-Informed ML"
        - name: Software
          tag: Software
        - name: Datasets and Benchmarking
          tag: Datasets
    design:
      columns: '1'
      view: community/citation_card
      background:
        image:
          filename: publicationsallbg.jpg
          filters:
            brightness: 0.15
          size: cover
          position: center
          parallax: true
---
