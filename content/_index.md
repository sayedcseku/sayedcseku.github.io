---
# Leave the homepage title empty to use the site title
title: ""
date: 2025-08-23
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/CV.pdf
    design:
      css_class: dark
      # Avatar customization
      avatar:
        size: medium  # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        My research develops machine learning systems that interpret complex patterns, anticipate future states, and support decision-making in safety-critical environments. I unify deep temporal learning with cross-domain intelligence across autonomous agents, simulation-based modeling, human–robot collaboration, and medical and visual AI.

        I began in biomedical image analysis—developing semi-supervised vessel segmentation for retinal images and multi-view Graph Convolutional Networks for mammography—which established my expertise in multimodal fusion and modeling under data scarcity. During my Ph.D. (funded by the Office of Naval Research), I focus on predictive maritime autonomy: building NavySim (a Unity-based multi-vessel simulator), ThreatMap (interpretable threat visualization), temporal intent models (HMMs, LSTMs, Transformers) achieving ~97% accuracy on seven maritime behaviors, and generative models (CVAE, TimeGAN, LSTM-GAN) for missing-data reconstruction and future-trajectory prediction. I also explore intent recognition in human–robot collaboration, applying embodied perspective-taking on robotic platforms.

        My goal is to advance anticipatory AI systems that understand their environment, anticipate future states, and act with reliability, transparency, and safety—bridging maritime security, healthcare, and robotics.
        
        [Download Research Statement (PDF)](/Files/Research%20Statement.pdf) · Please reach out to collaborate 😃
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      page_type: post
      count: 6
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
---
