---
title: 'Projects'
date: 2024-05-19
type: landing

design:
  spacing: '4rem'

sections:
  - block: collection
    id: selected-projects
    content:
      title: Selected Projects
      text: 'Flagship research spanning medical image analysis & medical AI systems, applied AI for autonomous systems, and generative deep learning.'
      count: 0
      filters:
        folders:
          - project
        featured_only: true
    design:
      view: article-grid
      fill_image: true
      columns: 2

  - block: collection
    id: foundational-research
    content:
      title: Earlier & Foundational Research
      text: 'Foundational investigations in medical computer vision, graph neural networks, and sequence modeling architectures.'
      count: 0
      filters:
        folders:
          - project
        exclude_featured: true
    design:
      view: article-grid
      fill_image: true
      columns: 3
      css_class: bg-slate-50 dark:bg-slate-900/50 py-12 rounded-2xl
---
