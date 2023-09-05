---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Welcome
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: collection
    id: featured
    content:
      title: Selected Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
      background:
        image: 
          # Name of image in `assets/media/`.
          filename: featuredbg.png
          # Apply image filters?
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.6
          #  Options are `cover` (default), `contain`, or `actual` size.
          size: cover
          # Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: true
          # Text color (true=light, false=dark, or remove for the dynamic theme color).
          # text_color_light: true
  - block: portfolio
    id: projects
    content:
      title: Projects
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
          tag: ml
        - name: Physics
          tag: phys
        - name: Software
          tag: comp
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
            brightness: 0.6
          #  Options are `cover` (default), `contain`, or `actual` size.
          size: cover
          # Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: true
          # Text color (true=light, false=dark, or remove for the dynamic theme color).
          # text_color_light: true
  - block: collection
    id: talks
    content:
      title: 'Selected Talks and Posters'
      subtitle: Complete list can be found at [raghavkansal.com/event](https://www.raghavkansal.com/event/)
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
      background:
        image: 
          # Name of image in `assets/media/`.
          filename: talksbg.jpg
          # Apply image filters?
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.6
          #  Options are `cover` (default), `contain`, or `actual` size.
          size: cover
          # Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: true
          # Text color (true=light, false=dark, or remove for the dynamic theme color).
          # text_color_light: true
  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Machine Learning + Particle Physics Researcher
          company: CMS Group / Duarte Lab, UC San Diego
          company_url: 'https://jduarte.physics.ucsd.edu'
          location: San Diego, USA
          date_start: '2019-09-01'
          date_end: ''
          description: |
              * Developing new graph generative models for sparse and irregular data like that prevalent in particle physics
              * Graph neural network (GNN) autoencoders for compression and anomaly detection, machine learning for particle flow reconstruction, Lorentz-group equivariant autoencoders, JetNet library for convenience and reproducibility in machine learning development in high energy physics
              * Developing and applying state-of-the-art GNN classifiers to set the most stringent constraints to date on double-Higgs production, allowing insight into the metastability of the universe
        - title: CERN Openlab Intern
          company: Machine Learning for Particle Physics Group, CERN
          company_url: 'https://cern.ch'
          location: Geneva, Switzerland
          date_start: '2019-06-01'
          date_end: '2019-08-01'
          description: |
              * Started our project on graph generative models for particle physics simulations, motivated primarily by the CMS experiment's new High Granularity Calorimeter (HGCAL)
        - title: Experimental Quantum Information Science Researcher
          company: Barreiro Lab, UC San Diego
          company_url: 'https://barreirolab.com'
          location: San Diego, USA
          date_start: '2017-06-01'
          date_end: '2019-06-01'
          description: |
              * Designed and implemented a setup for a quantum gas microscope (QGM) to image with single-site resolution
              * Generated 2D dynamic, arbitrarily arranged, sub-micron optical tweezers, integrated with the QGM, via two methods, using: 1) a Digital Micromirror Device (i.e. holography), and 2) an acousto-optic deflector
              * Characterized a high (0.8) Numerical Aperture objective for the QGM using OSLO optical simulations and point-spread function image analysis in Python
              * Using an FPGA device, outputted RF waveforms that modulate laser beams with parabolic spatial intensity in order to produce a Bose-Einstein Condensate
              * Programmed FPGA and C electronic devices, and created and (3D) printed mechanical mounts and electronics circuits for experimental use
        - title: Neurophysics Researcher
          company: Kleinfeld Lab, UC San Diego
          company_url: 'https://neurophysics.physics.ucsd.edu'
          location: San Diego, USA
          date_start: '2018-09-01'
          date_end: '2019-06-01'
          description: |
              * Used two-photon microscopy to measure pO2 in the mouse somatosensory cortex
              * Imaged the cortex to measure vasomotion relative to pO2
        - title: Software Intern
          company: Focus Analytics
          company_url: 'https://www.linkedin.com/company/retailnav/about/'
          location: Mumbai, India
          date_start: '2016-07-01'
          date_end: '2016-09-01'
          description: |
              * Interned at a software startup which has since been bought by Moka
              * Developed and deployed a location prediction SparkJava server with Cassandra and Redis databases
              * Implemented ML k-means clustering and SVM linear classification algorithms on location data
              * Wrote NodeJS servers and pages for receiving users’ predicted locations and displaying the live data on maps
              * Designed Cassandra and MySQL databases storing user tracking data, and wrote server APIs for accessing/updating, along with web panels for easy viewing of the data (using said APIs)
    design:
      columns: '2'
      background:
        image: 
          # Name of image in `assets/media/`.
          filename: expbg.jpg
          # Apply image filters?
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.6
          #  Options are `cover` (default), `contain`, or `actual` size.
          size: cover
          # Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: true
          # Text color (true=light, false=dark, or remove for the dynamic theme color).
          # text_color_light: true
  - block: accomplishments
    id: awards
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Awards'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url:
          date_end: "2024-05-01"
          date_start: "2023-05-01"
          description: "For searches for flavour changing neutral currents, ML for simulation, and self-supervised learning for jet classification."
          organization: Fermilab
          organization_url: https://www.fnal.gov
          title: Fermilab LPC Graduate Scholarship
          url: "https://lpc.fnal.gov/programs/graduate-scholars/index_2023.shtml"
        - certificate_url:
          date_end: ""
          date_start: "2021-11-24"
          description: "One of two recipients of this award, which 'honors outstanding graduate students in the Division of Physical Sciences who seek interdisciplinary approaches to problem solving and have a strong commitment to education, mentorship, and service.'"
          organization: UC San Diego Division of Physical Sciences
          organization_url: https://physicalsciences.ucsd.edu
          title: 2021-22 Carol and George Lattimer Award for Graduate Excellence
          url: ""
        - certificate_url:
          date_end: "2021-09-01"
          date_start: "2020-09-01"
          description: "For ML-based fast simulation software, ML techniques for reconstruction, compression, and anomaly detection tasks, and a boosted Higgs to WW tagger for precision measurements."
          organization: Fermilab
          organization_url: https://www.fnal.gov
          title: Fermilab LPC Artificial Intelligence Fellowship
          url: "https://lpc.fnal.gov/programs/ai-fellowships/index_2021.shtml"
        - certificate_url:
          date_end: ""
          date_start: "2019-08-01"
          description: "For the talk 'Deep Graph Neural Networks for Fast HGCAL Simulation'"
          organization: CERN
          organization_url: https://cern.ch
          title: CERN Openlab Summer Students Lightning Talks Award Runner-Up
          url: "https://home.cern/news/news/cern/cern-openlab-summer-student-programme-closes-lightning-talks"
        - certificate_url:
          date_end: ""
          date_start: "2019-06-01"
          description: "For the project 'HGCAL Fast Simulation with Graph Networks'"
          organization: IRIS-HEP
          organization_url: https://iris-hep.org
          title: 2019 IRIS-HEP Fellowship
          url: "https://iris-hep.org/fellows/RaghavKansal.html"
        - certificate_url: ""
          date_end: ""
          date_start: "2019-06-01"
          description: "Sole recipient of this prize, which is 'presented annually at commencement to a graduating physics student who is recognized for potential for a career in physics and a measure of experimental inquisitiveness.'"
          organization: UC San Diego Department of Physics
          organization_url: https://physics.ucsd.edu
          title: 2019 John Holmes Malmberg Prize
          url: "https://physics.ucsd.edu/Awards"
        - certificate_url: ''
          date_end: ""
          date_start: "2019-05-01"
          description: "One of 33 students from the departments of Mathematics, Physics and Chemistry 'recognized for excellence in academics and fundamental research'."
          organization: UC San Diego Division of Physical Sciences
          organization_url: https://physicalsciences.ucsd.edu
          title: "2018-2019 Physical Sciences Dean's Undergraduate Award for Excellence"
          url: ""
        - certificate_url: ''
          date_end: ""
          date_start: "2018-07-01"
          description: "For the project 'Arbitrary ultra-cold atomic lattices using holographic optical tweezers'"
          organization: UC San Diego Division of Physical Sciences
          organization_url: https://physicalsciences.ucsd.edu
          title: "2018 William A. Lee Undergraduate Research Award"
          url: ""
    design:
      columns: '2'
      background:
        image: 
          # Name of image in `assets/media/`.
          filename: awardsbg.jpg
          # Apply image filters?
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.6
          #  Options are `cover` (default), `contain`, or `actual` size.
          size: cover
          # Options include `left`, `center` (default), or `right`.
          position: center
          # Use a fun parallax-like fixed background effect on desktop? true/false
          parallax: true
          # Text color (true=light, false=dark, or remove for the dynamic theme color).
          # text_color_light: true
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      email: rkansal@ucsd.edu
      appointment_url: 'https://calendly.com/rkansal47'
      address:
        street: Wilson Hall, Rd a-1
        city: Batavia
        region: IL
        postcode: '60510'
        country: United States
        country_code: US
      # Automatically link email and phone or display as text?
      autolink: true
      coordinates:
        latitude: '37.4275'
        longitude: '-122.1697'
    design:
      columns: '2'
---
