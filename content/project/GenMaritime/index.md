---
title: "Joint Intent & Trajectory Prediction (MTITP GAN)"
date: 2026-05-01
featured: true
summary: Multi-task conditional generative network (MTITP-WGAN) jointly classifying vessel intent and forecasting future multi-modal trajectory distributions (Chapter 7, Ph.D. Dissertation).
links: []
tags:
  - Generative Adversarial Networks
  - Multi-Task Learning
  - Trajectory Prediction
  - Intent Recognition
  - Deep Learning
image:
  caption: "MTITP multi-task GAN architecture: joint past-intent classification, future-intent forecasting, and trajectory generation"
  focal_point: Smart
  preview_only: false
---

**Joint Intent and Trajectory Prediction (MTITP)** represents the headline generative contribution of Md Abu Sayed's doctoral dissertation (**Chapter 7**). Rather than treating intent recognition and trajectory forecasting as independent sequential pipelines, this work couples them inside a unified multi-task generative framework.

## Core Innovations & Architecture

- **MTITP-WGAN Framework**: Formulates a Multi-Task Intent and Trajectory Prediction Generative Adversarial Network trained with Wasserstein loss and gradient penalty (WGAN-GP) to eliminate mode collapse and generate realistic, multi-modal future paths.
- **Three-Pronged Joint Output**:
  1. **Past-Intent Classification**: Recognizes behavioral intent over historical encounter windows.
  2. **Future-Intent Forecasting**: Predicts forward-looking tactical intent transitions.
  3. **Intent-Conditioned Trajectory Synthesis**: Generates kinematically feasible future coordinate sequences conditioned on predicted intent.
- **Robustness Under Sensor Noise**: Evaluated extensively across simulator-generated benchmarks with varying noise regimes (Noiseless, Noisy 1, Noisy 2) and out-of-distribution adversarial encounters (herding, ramming, blocking).
- **Ablation & Baselines**: Rigorously benchmarked against MarITGAN v2 and non-adversarial variants (MTITP-L2) to isolate the exact contribution of adversarial loss to trajectory fidelity.

## Forthcoming Publications

- **Two pending journal manuscripts** are currently derived from this framework:
  - *Joint Multi-Task Intent and Trajectory Prediction for Autonomous Maritime Surface Vessels using Wasserstein GANs* (Target: *IEEE Transactions on Intelligent Transportation Systems (T-ITS)*)
  - *Generative Scenario Augmentation and Counterfactual Intent Analysis in Safety-Critical Maritime Encounters*
