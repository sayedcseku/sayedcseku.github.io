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
        url: uploads/CV_2025.pdf
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
        My research focuses on developing **intelligent systems that can perceive, predict, and adapt in dynamic environments**, with applications ranging from **maritime security and simulation** to **medical image analysis and computer vision**.

        ## Research Background
        I began my research journey working on **medical image processing**, particularly the segmentation of retinal blood vessels and the detection of breast cancer from mammograms. In these projects, I explored **deep learning, graph convolution networks, and hybrid supervised–unsupervised techniques** to enhance the accuracy of disease detection. This early work shaped my appreciation for the power of **computer vision and AI** to support critical human-centered decision-making in healthcare.

        ## Current Research
        As a Ph.D. student in **Computer Science and Engineering** at the University of Nevada, Reno, my current research centers on **machine learning and simulation for maritime intent recognition and threat prediction**. I developed **NavySim**, a multi-vessel naval simulation engine, and designed algorithms that integrate **Hidden Markov Models, LSTMs, and transformer-based approaches** for predicting vessel intentions in uncertain and adversarial environments. My work has led to multiple publications in **top IEEE conferences and journals**, and has been presented internationally in Europe.

        ## Future Vision
        Looking forward, I aim to **bridge my experience in medical image analysis, computer vision, and maritime AI** to push forward the development of **trustworthy, interpretable, and cross-domain intelligent systems**. Specifically:
        - In **maritime security**, I will continue advancing **simulation-driven learning frameworks** and **robust intent recognition models** for safety-critical applications.
        - In **medical imaging**, I plan to return to my earlier interests by leveraging **deep learning and computer vision** for early disease detection, cross-modal reasoning, and explainable AI for healthcare.
        - In **computer vision and AI at large**, I am motivated to explore how **simulation and data-driven methods can work together** to create models that are both accurate and human-interpretable.

        ## Impact
        Across these domains, my ultimate goal is to design **AI systems that not only achieve state-of-the-art performance, but also enhance human trust, awareness, and decision-making**. By combining insights from **maritime simulation, computer vision, and medical imaging**, I aim to contribute to both **scientific innovation** and **real-world problem-solving**.
        
        Please reach out to collaborate 😃
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
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
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
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!
        
        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
