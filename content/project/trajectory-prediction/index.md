---
title: "Maritime Trajectory Prediction & State Estimation"
date: 2026-04-15
featured: true
summary: Systematic empirical evaluation of classical Bayesian filters and state estimators for multi-vessel trajectory prediction across horizons and noise regimes (Chapter 6, Ph.D. Dissertation).
links: []
tags:
  - Trajectory Prediction
  - Bayesian Filtering
  - Kalman Filters (EKF / UKF)
  - State Estimation
  - Maritime Autonomy
image:
  caption: "Empirical comparison of EKF-CTRV vs. UKF-CTRV trajectory forecasts and horizon-wise MAE error curves (Chapter 6)"
  focal_point: Smart
  preview_only: false
---

**Maritime Trajectory Prediction & Bayesian State Estimation** forms the foundational empirical benchmarking contribution of Md Abu Sayed's doctoral dissertation (**Chapter 6**; *TrajectoryKF*). 

Before deploying complex deep generative models, operational autonomy systems require establishing the exact performance boundary of classical Bayesian filters and kinematics estimators. This project provides a comprehensive, fine-grained empirical study comparing six canonical filter architectures across multi-vessel encounter dynamics.

## Evaluated Filter Architectures

1. **Constant Velocity (CV) Baseline**: Linear state propagation under Gaussian motion assumption.
2. **Standard Unscented Kalman Filter (UKF-4D)**: Nonlinear sigma-point propagation with standard 4D kinematic state `[x, y, v_x, v_y]`.
3. **UKF with 5D Constant-Velocity State (UKF-5D-CV)**: Augments the state with heading (θ) for coordinated forward extrapolation.
4. **Asymmetric UKF with Acceleration State (UKF-CA-6D)**: Models constant acceleration `[a_x, a_y]` to capture rate changes during maneuvering.
5. **Extended Kalman Filter with Constant Turn Rate & Velocity (EKF-CTRV)**: Analytic Jacobian linearization of circular arc kinematics `[x, y, v, θ, ω]`.
6. **UKF-CTRV**: Deterministic sigma-point propagation through exact CTRV nonlinear dynamics.

## Key Findings & Research Questions

- **Nonlinear Dynamics & Sigma-Point Propagation**: When motion models are linear, sigma-point propagation collapses to the closed-form Kalman update; UKF provides clear benefits only when unprojected heading or turn rates are actively estimated.
- **Observability & Covariance Divergence**: Because turn rate (ω) is not directly measured by radar/AIS and must be inferred from sequential coordinates, UKF-CTRV covariances diverge during long-horizon predict-only phases (T_pred ≥ 10), whereas EKF-CTRV remains numerically bounded.
- **Horizon Limits of Kinematic Models**: Across four experiment horizons (T_obs ∈ {20, 40}, T_pred ∈ {5, 10, 20}), classical CTRV models maintain competitive performance on benign and crossing encounters (ADE < 1.5 m) but diverge sharply on adversarial maneuvers (herding, ramming), proving that pure kinematic filters cannot substitute for tactical intent understanding.
- **Foundation for Chapter 7**: Directly motivates the multi-task intent-conditioned generative architecture (MTITP GAN) developed in Chapter 7.
