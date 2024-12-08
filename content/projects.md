---
# Leave the homepage title empty to use the site title
title: Projects
date: 2022-10-24
type: landing

sections:
  - block: portfolio
    id: projects
    content:
      title: Projects
      subtitle: "Click the projects below to see related publications, talks, and more info." 
      filters:
        folders:
          - project
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
        - name: ML
          tag: ML
        - name: High Energy Physics
          tag: HEP
        - name: Quantum Information
          tag: QIS
        - name: Software
          tag: Software
      sort_by: "Weight"
      sort_ascending: true
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: masonry
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
      background:
        image: 
          # Name of image in `assets/media/`.
          filename: projectsbg2.jpg
          # Apply image filters?
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.2
          #  Options are `cover` (default), `contain`, or `actual` size.
          size: cover
          # Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: true
          # Text color (true=light, false=dark, or remove for the dynamic theme color).
          # text_color_light: true
---