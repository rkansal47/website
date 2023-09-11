---
title: Particle Cloud Generation with Message Passing GANs

event: APS April Meeting 2022
event_url: https://meetings.aps.org/Meeting/APR22/Session/B10.4

talk_type: Poster

location: 'New York'
location_link: https://meetings.aps.org/Meeting/APR22/Content/4194

summary: ''
abstract: "There has been significant development recently in generative models for accelerating LHC simulations. Work on simulating jets has primarily used image-based representations, which tend to be sparse and of limited resolution. We advocate for the more natural 'particle cloud' representation of jets, i.e. as a set of particles in momentum space, and discuss four physics- and computer-vision-inspired metrics: (1) the 1-Wasserstein distance between high- and low-level feature distributions; (2) a new Fréchet ParticleNet Distance; (3) the coverage; and (4) the minimum matching distance as means of quantitatively and holistically evaluating generated particle clouds. We then present our new message-passing generative adversarial network (MPGAN), which has excellent performance on gluon, top quark, and lighter quark jets on all metrics, validated against real samples via bootstrapping as well as existing point cloud generative models, and shows promise for use in high energy physics."

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2022-04-10T08:00:00Z"
# <!-- date_end: "2030-06-01T15:00:00Z" -->
all_day: false

# Schedule page publish date (NOT talk date).
# publishDate: "2017-01-01T00:00:00Z"

authors: []
tags: ["ML", "Simulation", "HEP", "Equivariant and Physics-Informed ML"]

# Is this a featured talk? (true/false)
featured: false

links:
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
url_poster: ""

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides:

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects:
- fast-sim
---
