---
title: "Breast Cancer Detection via Multimodal Fusion with GCN"
date: 2022-01-01
summary: Graph Convolutional Neural Networks with Mask-RCNN backend for bilateral and ipsilateral mammogram fusion, malignancy detection, and semantic segmentation.
links:
  - icon: brands/github
    name: ContrastMammogram
    url: https://github.com/sayedcseku/ContrastMammogram
tags:
  - Medical Imaging
  - Deep Learning
  - Graph Neural Networks
  - PyTorch
image:
  caption: "Multimodal mammogram analysis with GCN for mass detection"
  focal_point: Smart
  preview_only: false
---

**Breast Cancer Detection via Multimodal Fusion with GCN** builds Graph Convolutional Neural Network models to reason over bilateral and ipsilateral mammogram views for improved malignancy detection and semantic segmentation.

## Key Contributions

- **Multimodal Fusion**: Developed GCN models with Mask-RCNN backend to fuse information across multiple mammogram views, capturing bilateral and ipsilateral cues for architectural distortion analysis.

- **Architectural Distortion Augmentation**: Implemented augmentation strategies to improve sensitivity to temporal and structural breast tissue changes over multiple clinical visits.

- **Mass Detection & Segmentation**: Models perform both malignancy detection and semantic segmentation of suspicious regions, supporting radiologist decision-making.

- **Course Context**: Initial development in CS 791 (Mass Detection in Mammograms) at UNR; extends expertise in multi-view fusion and spatial–temporal pattern learning from retinal imaging to mammography.
