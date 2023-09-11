---
# Leave the homepage title empty to use the site title
title: Selected Publications
date: 2022-10-24
type: landing

sections:
  - block: collection
    id: select-talks
    content:
      title: 'Selected Talks and Posters'
      filters:
        folders:
          - event
        featured_only: true 
      archive:
        text: "See all" 
        link: /talks
      count: 100
    design:
      columns: '1'
      view: community/event_card
      background:
        image: 
          # Name of image in `assets/media/`.
          filename: talksbg.jpg
          # Apply image filters?
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.9
          #  Options are `cover` (default), `contain`, or `actual` size.
          size: cover
          # Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: true
          # Text color (true=light, false=dark, or remove for the dynamic theme color).
          # text_color_light: true
---
