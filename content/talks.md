---
# Leave the homepage title empty to use the site title
title: Talks and Posters
date: 2022-10-24
type: landing

sections:
  - block: portfolio
    id: featured
    content:
      title: Talks and Posters
      filters:
        folders:
          - event
        featured_only: false
      archive:
        enable: false
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
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
        - name: Quantum Information
          tag: QIS
        - name: Video
          tag: Video
        # - name: Datasets and Benchmarking
        #   tag: Datasets
    design:
      columns: '1'
      view: community/event_list
      background:
        image: 
          # Name of image in `assets/media/`.
          filename: talksbg.jpg
          # Apply image filters?
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.1
          #  Options are `cover` (default), `contain`, or `actual` size.
          size: cover
          # Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: true
          # Text color (true=light, false=dark, or remove for the dynamic theme color).
          # text_color_light: true
---
