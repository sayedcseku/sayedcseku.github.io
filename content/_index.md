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
      buttons:
        - text: Academic CV
          url: uploads/CV_Academic.pdf
        - text: Industry Resume
          url: uploads/Resume_Industry.pdf
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
      subtitle: 'Cardiovascular AI & CDSS · Joint Intent Recognition & Trajectory Prediction · Deep Learning'
      text: |-
        My research focuses on cardiovascular AI, medical image analysis, and multi-agent intent recognition. At the University of Miami, I build multimodal clinical decision support systems that integrate IVUS, OCT, and angiography with biomechanical simulations for coronary interventions. During my doctoral studies at the University of Nevada, Reno, I developed simulation engines, feature attribution methods, and generative sequence models for trajectory prediction and intent recognition in autonomous systems.

        <div class="research-grid not-prose">
        <div class="research-card"><span class="ico">🫀</span><h3>Cardiovascular AI &amp; CDSS <span class="tag">· Current</span></h3><p>Multimodal deep learning integrating HD-IVUS, OCT, and angiography with biomechanical simulation for clinical decision support in PCI.</p></div>
        <div class="research-card"><span class="ico">🛰️</span><h3>Joint Intent Recognition &amp; Trajectory Prediction <span class="tag tag-muted">· PhD</span></h3><p>Doctoral research at UNR developing the NavySim simulation engine, feature attribution methods (CPFI/TFIS), and multi-task generative models (MTITP) for intent and trajectory forecasting.</p></div>
        <div class="research-card"><span class="ico">🧠</span><h3>Foundational &amp; Applied AI</h3><p>Research across retinal vessel segmentation, mammography analysis with graph neural networks, and human–robot collaboration studies.</p></div>
        </div>
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
      archive:
        enable: true
        text: 'View all publications →'
        link: 'publication/'
    design:
      view: citation
      css_class: bg-slate-50 dark:bg-slate-900/40

  # Projects preview: Visual showcase
  - block: collection
    id: projects
    content:
      title: Selected Projects
      subtitle: 'Research & development across cardiovascular AI, maritime autonomy, generative modeling, and robotics'
      text: ''
      count: 6
      filters:
        folders:
          - project
      order: desc
      archive:
        enable: true
        text: 'View all projects →'
        link: 'projects/'
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
