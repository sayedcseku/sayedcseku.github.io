---
title: "NavySim: A Multi-Vessel Simulation and Analysis Engine for Naval Domains"
authors:
- Md Abu Sayed
- Korben DiArchangel
- Mayamin Hamid Raha
- Parvaneh Aliniya
- Monica Nicolescu
- Mircea Nicolescu
- Sushil Louis

date: 2024-08-28

publication_types: ['paper-conference']
publication: "2024 IEEE Conference on Games (CoG)"
# doi: "10.1109/CoG60054.2024.10645561"

abstract: In this paper, we focus on the field of maritime simulation games, also known as serious games or simulators, which serve as a vital tool for maritime education and training. These simulations offer a controlled and risk-free platform to mimic real-world situations, thereby aiding seafarers in learning essential skills such as ship maneuverability, collision prevention, and understanding other naval agents’ intentions. We present an implementation of a Unity-based naval simulator that enables the development of complex, multi-vessel navigation scenarios and provides multiple key capabilities relevant to the naval domain. First, the agent vessels are equipped with mathematical models to assess their capabilities and vulnerabilities. Second, a vulnerability heatmap is developed to illustrate the sensor and defense coverage of an agent or a group of agents. Third, a Closest Point of Approach (CPA) based action heatmap is developed to explore potential threats from the surrounding agents. Furthermore, these heatmaps are fused into a threat heatmap that encodes in real time an agent’s overall coverage and potential threats. In addition, vessel agents are equipped with Hidden Markov Model-based intent recognition models, to analyze the behavior of other agents around them. This paper describes the naval simulator with its capabilities and illustrates its main capabilities in various naval scenarios.

# Summary. An optional shortened abstract.
summary: We introduce a Unity-based naval simulator for maritime training that supports complex multi-vessel scenarios, real-time threat assessment, and intent recognition. The system models vessel capabilities, renders vulnerability and CPA-based action heatmaps, fuses them into a dynamic threat map, and uses HMMs to infer other agents’ intentions.

tags:
  - Maritime Simulation Engine
  - Hidden Markov Model
  - Intent Recognition
  - Serious Game

# Display this page in the Featured widget?
featured: true

# Standard identifiers for auto-linking
hugoblox:
  ids:
    doi: 10.1109/CoG60054.2024.10645561

# Custom links
links:
  - type: pdf
    url: ""
  - type: code
    url: ""
  - type: dataset
    url: ""
  - type: slides
    url: https://docs.google.com/presentation/d/171YHcQB756reoXl0uMMFa4yRniJJ4Y5Q/edit?usp=sharing&ouid=105064277540442270443&rtpof=true&sd=true
  - type: source
    url: ""
  - type: video
    url: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: [**IEEE**](https://ieeexplore.ieee.org/abstract/document/10645561)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
