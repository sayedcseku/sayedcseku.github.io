---
title: "Retinal Image Analysis & Local Haar Pattern (LHP) Descriptor"
date: 2018-06-01
summary: Segmentation pipelines and Local Haar Pattern descriptor for retinal fundus images, achieving state-of-the-art accuracy on DRIVE, STARE, and CHASE_DB1.
links:
  - icon: brands/github
    name: retinalVesselSegmentation
    url: https://github.com/sayedcseku/retinalVesselSegmentation
tags:
  - Medical Imaging
  - Computer Vision
  - Retinal Vessel Segmentation
  - MATLAB
image:
  caption: "Retinal vessel segmentation with Local Haar Pattern descriptor"
  focal_point: Smart
  preview_only: false
---

**Retinal Image Analysis & Local Haar Pattern (LHP)** develops automated methods to segment retinal blood vessels from color fundus photographs—a critical diagnostic procedure in ophthalmology. The work addresses the challenge of robust vessel segmentation in the presence of pathological lesions.

## Key Contributions

- **Local Haar Pattern (LHP) Descriptor**: Proposed a novel descriptor to capture domain-specific vascular and lesion structures in retinal images. LHP uniquely describes vessel pixels even in the presence of pathology.

- **Pipeline**: Developed vessel enhancement, initial segmentation via multi-scale line detector, feature extraction using LHP, and morphological post-processing. SVM and Random Forest classifiers perform vessel vs. non-vessel classification.

- **State-of-the-Art Results**: The method achieves 96% accuracy on DRIVE, 96% on STARE, and 95% on CHASE_DB1—outperforming contemporary supervised and semi-supervised baselines. Combines supervised and unsupervised approaches for pathology-robust segmentation.

## Related Publications

- **An Innovate Approach for Retinal Blood Vessel Segmentation Using Mixture of Supervised and Unsupervised Methods** — IET Image Processing 2021
- **A Semi-Supervised Approach to Segment Retinal Blood Vessels in Color Fundus Photographs** — AIME 2019
- **Retinal Blood Vessel Segmentation: A Semi-Supervised Approach** — IbPRIA 2019
