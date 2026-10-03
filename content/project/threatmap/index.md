---
title: "ThreatMap: Maritime Situational Awareness"
date: 2021-08-01
summary: Heatmap framework that fuses sensor coverage, vulnerability fields, and CPA-based threat estimates for real-time maritime risk visualization.
links: []
tags:
  - Maritime AI
  - Visualization
  - Python
  - Unity
  - Shader
image:
  caption: "ThreatMap heatmap showing threat levels around naval vessels"
  focal_point: Smart
  preview_only: false
---

**ThreatMap** is an interpretable, real-time visualization framework for maritime risk assessment. It supports operator trust by providing spatial context behind mathematical model-based predictions through an intuitive green-to-red heatmap representation.

## Key Features

- **Fused Threat Model**: Combines (1) sensor and weapon coverage, (2) vulnerability fields from blind zones and pose, and (3) CPA/TCPA-based threat estimates from kinematic features.

- **Real-Time Rendering**: Custom Unity shaders render dynamic heatmaps directly on the simulation environment, updating in real time as vessel positions and intents evolve.

- **Integration**: Fully integrated into NavySim and connected to intent recognition models. The heatmap encodes an agent's overall coverage and potential threats from surrounding vessels.

- **Decision Support**: Gives decision-makers an intuitive understanding of evolving threats and the factors driving model outputs, supporting on-water and simulation-driven analysis.

## Related Publications

- **ThreatMap: A Framework for Enhancing Security Awareness and Decision-Making for Naval Agents** — International Conference on Harbor, Maritime and Multimodal Logistic Modeling & Simulation (HMS) 2024
- **NavySim: A Multi-Vessel Simulation and Analysis Engine for Naval Domains** — IEEE CoG 2024 (integrated ThreatMap)
