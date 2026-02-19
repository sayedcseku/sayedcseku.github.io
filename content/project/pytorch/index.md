---
title: "NavySim: Multi-Vessel Simulation Engine"
date: 2022-06-01
summary: Unity-based naval simulator with physics-consistent multi-agent scenarios, real-time threat heatmaps, and ML-driven intent recognition for maritime research.
links: []
tags:
  - Simulation
  - Maritime AI
  - Unity
  - Intent Recognition
  - C#
image:
  caption: "NavySim multi-vessel maritime scenarios with heatmap visualization"
  focal_point: Smart
  preview_only: false
---

**NavySim** is a Unity-based multi-vessel simulation and analysis engine developed for advanced naval research. It enables the creation of complex, physics-consistent maritime scenarios where multiple vessels interact in realistic environments.

## Key Features

- **Scenario Generation Pipeline**: Built a scenario-generation pipeline enabling physics-consistent multi-agent maritime interactions with configurable vessel dynamics, sensing ranges, and defensive coverage areas.

- **Threat & Vulnerability Heatmaps**: Integrated real-time CPA/TCPA-based action heatmaps and vulnerability heatmaps (sensor/weapon coverage) via custom Unity shaders. These fuse into a unified threat heatmap for situational awareness.

- **ML Integration**: Wired HMM/LSTM intent recognition models through a TCP pipeline, enabling real-time prediction of vessel intent and threat-aware decision support directly within the simulation.

- **Deployment-Ready**: Designed for on-water deployment collaboration with Huntington Ingalls Industries and supports benchmarking of early intent prediction algorithms.

## Related Publications

- **NavySim: A Multi-Vessel Simulation and Analysis Engine for Naval Domains** — IEEE Conference on Games (CoG) 2024
- **NavySim 2.0: Enhanced Multi-Vessel Simulation and Analysis Engine for Advanced Naval Research** — IEEE Transactions on Games 2025 (Accepted)
