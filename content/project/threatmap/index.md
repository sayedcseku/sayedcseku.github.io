---
title: "ThreatMap: Maritime Situational Awareness"
date: 2023-12-05
summary: Real-time heatmap framework fusing sensor coverage, vulnerability fields, and CPA-based threat estimates for naval situational awareness (2021–2023).
links: []
tags:
  - Maritime AI
  - Situational Awareness
  - Heatmap Visualization
  - Unity
  - C# / Shaders
image:
  caption: "ThreatMap dynamic risk heatmap in naval simulation (HMS 2024 / M.S. Thesis)"
  focal_point: Smart
  preview_only: false
---

**ThreatMap: Maritime Situational Awareness (2021–2023)** is an interpretable, real-time spatial risk visualization framework developed as part of Md Abu Sayed's M.S. thesis research at the University of Nevada, Reno, and published at HMS 2024. It translates complex kinematic relations and vessel capabilities into an intuitive green-to-red threat surface directly within maritime environments.

## Key Features

- **Fused Threat Model**: Combines (1) sensor and weapon coverage, (2) vulnerability fields from blind zones and pose, and (3) CPA/TCPA-based threat estimates from kinematic features.

- **Real-Time Rendering**: Custom Unity shaders render dynamic heatmaps directly on the simulation environment, updating in real time as vessel positions and intents evolve.

- **Integration**: Fully integrated into NavySim and connected to intent recognition models. The heatmap encodes an agent's overall coverage and potential threats from surrounding vessels.

- **Decision Support**: Gives decision-makers an intuitive understanding of evolving threats and the factors driving model outputs, supporting on-water and simulation-driven analysis.

## Related Publications

- **ThreatMap: A Framework for Enhancing Security Awareness and Decision-Making for Naval Agents** — International Conference on Harbor, Maritime and Multimodal Logistic Modeling & Simulation (HMS) 2024
- **NavySim: A Multi-Vessel Simulation and Analysis Engine for Naval Domains** — IEEE CoG 2024 (integrated ThreatMap)
