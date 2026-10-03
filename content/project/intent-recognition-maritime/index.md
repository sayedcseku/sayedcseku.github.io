---
title: "Intent Recognition for Maritime Autonomy"
date: 2022-06-01
summary: Deep and probabilistic intent classifiers (HMMs, LSTMs, Transformers) for early vessel behavior prediction in adversarial maritime scenarios.
links: []
tags:
  - Intent Recognition
  - Maritime AI
  - Deep Learning
  - Sequence Modeling
image:
  caption: "Feature-aware intent classification for maritime vessel behaviors"
  focal_point: Smart
  preview_only: false
---

**Intent Recognition for Maritime Autonomy** develops temporal and deep learning models for early prediction of vessel behavior in complex maritime scenarios. The work addresses the challenge of recognizing intent despite sparse, noisy, and adversarial observations—critical for safety-critical decision support on naval platforms.

## Key Contributions

- **Feature-Aware Models**: Designed architectures incorporating bearing-rate, CPA/TCPA, and motion derivatives to improve early prediction under sparse and noisy observations. LSTM, Bi-LSTM, and Transformer classifiers achieve ~97% accuracy on seven maritime behaviors using only initial trajectory segments.

- **Sliding-Window Formulation**: Extended to rolling-threat prediction with sliding-window classification, reaching 81–88% multiclass accuracy and ~90% hostile–benign accuracy with short 20-second observation windows.

- **Probabilistic Baseline**: Built HMM-based intent models for interpretable, uncertainty-aware predictions that integrate with threat visualization systems.

- **Integration**: Models are deployed within NavySim and support real-time threat-aware decision-making for naval agents.

## Related Publications

- **Feature-Aware Deep Learning for Maritime Intent Recognition** — IEEE FMLDS 2025 (forthcoming)
- **Early Classification of Intentions for Maritime Domains Using Deep Learning Models** — IEEE CASE 2025
- **Proactive Maritime Threat Prediction: Vessel Intent Classification with LSTMs and Transformers Using a Sliding Window Approach** — IEEE CASE 2025 (with A. Meepaganithage et al.)
