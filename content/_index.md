---
# Leave the homepage title empty to use the site title
title: ""
date: 2025-08-23
type: landing

design:
  spacing: "5rem"

sections:
  # Hero: Bold, dark intro
  - block: resume-biography-3
    content:
      username: admin
      text: ""
      button:
        text: Download CV
        url: uploads/CV.pdf
    design:
      css_class: dark
      avatar:
        size: large
        shape: circle
      background:
        color: black
        image:
          filename: stacked-peaks.svg
          filters:
            brightness: 0.4
            contrast: 1.1
          size: cover
          position: center
          parallax: false

  # Research: Clean section with soft accent
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: 'Predictive AI · Intent Recognition · Maritime Autonomy'
      text: |-
        My research develops machine learning systems that interpret complex patterns, anticipate future states, and support decision-making in safety-critical environments. I unify deep temporal learning with cross-domain intelligence across autonomous agents, simulation-based modeling, human–robot collaboration, and medical and visual AI.

        I began in biomedical image analysis—developing semi-supervised vessel segmentation for retinal images and multi-view Graph Convolutional Networks for mammography—which established my expertise in multimodal fusion and modeling under data scarcity. During my Ph.D. (funded by the Office of Naval Research), I focus on predictive maritime autonomy: building **NavySim** (a Unity-based multi-vessel simulator), **ThreatMap** (interpretable threat visualization), temporal intent models (HMMs, LSTMs, Transformers) achieving ~97% accuracy on seven maritime behaviors, and generative models (CVAE, TimeGAN, LSTM-GAN) for missing-data reconstruction and future-trajectory prediction. I also explore intent recognition in human–robot collaboration, applying embodied perspective-taking on robotic platforms.

        My goal is to advance anticipatory AI systems that understand their environment, anticipate future states, and act with reliability, transparency, and safety—bridging maritime security, healthcare, and robotics.

        [Download Research Statement (PDF)](/Files/Research%20Statement.pdf) · Please reach out to collaborate 😃
    design:
      columns: '1'
      css_class: bg-slate-50 dark:bg-slate-900/50

  # Featured publications: Highlighted grid
  - block: collection
    id: papers
    content:
      title: Featured Publications
      subtitle: ''
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
      css_class: bg-white dark:bg-slate-950

  # Recent publications: Citation list
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
      css_class: bg-slate-50 dark:bg-slate-900/40

  # Projects preview: Visual showcase
  - block: collection
    id: projects
    content:
      title: Selected Projects
      subtitle: 'Research & development across maritime AI, medical imaging, and simulation'
      text: ''
      count: 4
      filters:
        folders:
          - project
      order: desc
    design:
      view: article-grid
      fill_image: true
      columns: 2
      css_class: bg-white dark:bg-slate-950

  # Talks & events
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      subtitle: 'Conference presentations'
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
      css_class: bg-slate-50 dark:bg-slate-900/50

  # News: Timely updates
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      page_type: post
      count: 6
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      offset: 0
      order: desc
    design:
      view: date-title-summary
      css_class: bg-white dark:bg-slate-950
      spacing:
        padding: [2rem, 0, 2rem, 0]
---
