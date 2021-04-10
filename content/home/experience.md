---
# An instance of the Experience widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: experience

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 60
active: true

title: Experience
subtitle:

design:
  background:
    # Name of image in `assets/media/`.
    image: expbg.jpg
    # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.
    image_darken: 0.4
    #  Options are `cover` (default), `contain`, or `actual` size.
    image_size: cover
    # Options include `left`, `center` (default), or `right`.
    image_position: center
    # Use a fun parallax-like fixed background effect on desktop? true/false
    image_parallax: true
    # Text color (true=light, false=dark, or remove for the dynamic theme color).

# Date format for experience
#   Refer to https://wowchemy.com/docs/customization/#date-format
date_format: Jan 2006

# Experiences.
#   Add/remove as many `experience` items below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
experience:
  - title: Machine Learning + Particle Physics Researcher
    company: Duarte Lab, UC San Diego
    company_url: 'https://jduarte.physics.ucsd.edu'
    location: San Diego, USA
    date_start: '2019-09-01'
    date_end: ''
    description: |
        * Developing new graph generative models for sparse and irregular data like that in particle physics
        * Using new deep graph neural network classifiers to set the most stringent constraints to date on double-Higgs production, allowing insight into the metastability of the universe
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


---
