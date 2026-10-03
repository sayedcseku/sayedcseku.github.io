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
        My research focuses on two core domains: **Cardiovascular AI & CDSS** and **Joint Intent Recognition and Trajectory Prediction**. Both are driven by a single methodological spine: deep learning for prediction and decision support under noisy, incomplete, or high-stakes observations—using temporal sequence modeling, generative architectures, and explainability to anticipate complex behaviors and guide critical actions.

        <div class="research-grid not-prose">
        <div class="research-card"><span class="ico">🫀</span><h3>Cardiovascular AI &amp; CDSS <span class="tag">· Current</span></h3><p>At the University of Miami's Center for Digital Cardiovascular Innovations, I develop multimodal agentic AI fusing HD-IVUS, OCT, and Angiography with biomechanical simulation for procedural decision support in PCI.</p></div>
        <div class="research-card"><span class="ico">🛰️</span><h3>Joint Intent Recognition &amp; Trajectory Prediction <span class="tag tag-muted">· PhD</span></h3><p>My doctoral dissertation at UNR: the NavySim multi-vessel simulator, explainable feature attribution (CPFI/TFIS), and MTITP—a multi-task GAN jointly predicting vessel intent and intent-conditioned trajectories.</p></div>
        <div class="research-card"><span class="ico">🧠</span><h3>Foundational &amp; Applied AI</h3><p>Retinal vessel segmentation, multi-view mammography GCNs, and human–robot collaboration—translating anticipatory and generative deep learning to high-impact decision-support problems.</p></div>
        </div>

        My goal is trustworthy, anticipatory AI that understands dynamic environments and acts with reliability and transparency. Please reach out to collaborate 😃
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
