---
title: Publications
cms_exclude: true
date: 2022-10-24
type: landing

# The wowchemy theme has hard-coded `eq .Type "publication"` checks in
# page_metadata, page_header, layouts/publication/single.html, etc. Cascade
# `type: publication` to all child pages so those checks fire (the URL still
# comes from the `publications/` folder name).
cascade:
  type: publication

sections:
  - block: portfolio
    id: featured
    content:
      title: Publications
      text: |
        <p style="font-weight: normal; font-size: 0.8rem; opacity: 0.85;">
        Note: As a member of the CMS Collaboration, I am an author on all CMS publications.
        Below I list only those CMS publications to which I made significant direct contributions.
        </p>
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
        - name: "Equivariant / Physics-Informed ML"
          tag: "Equivariant and Physics-Informed ML"
        - name: "Biology"
          tag: "Biology"
        - name: "Higgs"
          tag: "Higgs"
        - name: "CMS"
          tag: "CMS"
        - name: "Simulation"
          tag: "Simulation"
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
