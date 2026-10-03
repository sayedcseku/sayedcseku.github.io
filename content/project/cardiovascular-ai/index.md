---
title: "Cardiovascular AI: Multimodal Imaging (IVUS/OCT & Angiography) & Agentic Decision Support"
subtitle: "June 2026 – Present"
date: 2026-06-08
featured: true
summary: Fusing IVUS, OCT, and X-ray Angiography for coronary lesion analysis and agentic clinical decision support in percutaneous coronary interventions (PCI).
tags:
  - Medical Image Analysis
  - Medical AI Systems
  - Cardiovascular AI
  - Multimodal Medical Imaging
  - IVUS / OCT
  - X-Ray Angiography
  - Agentic Decision Support
  - Deep Learning
image:
  caption: "Multimodal cardiovascular analysis fusing IVUS, OCT, and Angiography within an agentic decision support pipeline"
  focal_point: Smart
  preview_only: false
---

At the Center for Digital Cardiovascular Innovations, University of Miami Miller School of Medicine (directed by Dr. Yiannis S. Chatzizisis), this project develops deep learning models and clinical decision support systems (CDSS) for percutaneous coronary interventions (PCI).

## Multimodal Image Analysis: IVUS, OCT & Angiography

The system combines complementary imaging modalities across scales:

- **High-Definition IVUS (HD-IVUS & NIRS-IVUS)**: Deep multi-task ConvNeXt-U-Net networks segmenting lumen, vessel wall (external elastic membrane), and plaque composition (calcium, fibrous, fibrolipidic) across 40,000+ expert-annotated IVUS frames.
- **Intracoronary Optical Coherence Tomography (OCT)**: High-resolution (10–15 µm) optical profiling capturing thin-cap fibroatheromas (TCFA), macrophage infiltration, and acute post-stent malapposition.
- **X-Ray Coronary Angiography (Luminography & QCA)**: Macroscopic vessel roadmapping, bifurcation anatomy tracking, and automated co-registration with pullback cross-sections.

![Multitask ConvNeXt-U-Net Architecture for HD-IVUS](architecture.png)
*Figure: Multitask ConvNeXt-U-Net architecture with multi-resolution stages (L0–L3) and specialized heads for radial-distance-weighted denoising, lumen/EEM boundary delineation, and plaque tissue characterization.*

## Clinical Decision Support System (CDSS)

The clinical decision support system integrates automated segmentation outputs with biomechanical simulation for procedural planning:

- **Automated Calcium Phenotyping**: Quantitative assessment of calcium arc, longitudinal length, and radial depth to compute standardized calcium fracture risk scores.
- **Lesion Preparation Assessment**: Evaluates lesion preparation strategies (non-compliant balloons, intravascular lithotripsy, rotational atherectomy) based on plaque morphology and calcification.
- **Virtual Stenting Simulation**: Couples finite element analysis (FEA) and learned surrogate models across 1,200 lesion phenotypes to estimate stent expansion and reduce under-expansion risks.

## Related Manuscripts & Clinical Studies

- **Deep Learning Model for Multi-Class Segmentation of High-Definition Intravascular Ultrasound** — Under review at *Scientific Reports* (2026)
- **Head-to-Head Comparison of Coronary Artery Bifurcation Stenting Strategies: A Virtual Clinical Study** — Under review at *JACC: Cardiovascular Interventions* (2026)
- **Head-to-Head Comparison of Latest Intracoronary Imaging Modalities** — Submitted to *JACC: Cardiovascular Interventions* (2026)
