---
layout: page
title: GP surrogates for EV-charging feasibility
description: Gaussian-process surrogates that replace repeated AC power-flow solves when screening EV charging on power grids. IIT Roorkee.
importance: 2
category: research
---

**Department of Electrical Engineering, IIT Roorkee, February – April 2026.** Advisor: Prof. Parikshit Pareek.

Checking whether a grid can accept a given pattern of EV charging normally means solving the AC power-flow equations for every operating point. This project replaced those repeated solves with Gaussian-process (GP) surrogates.

- **Data.** I generated AC power-flow datasets in Julia across a range of loading conditions.
- **Surrogates.** GPU-accelerated GP regression models (BoTorch, CUDA) with a squared-exponential kernel reached errors of about 10<sup>-5</sup> p.u. in voltage magnitude and 10<sup>-4</sup> rad in voltage angle.
- **Screening.** The GP predictive uncertainty is used to screen for voltage-constraint violations, delivered through an interactive feasibility-analysis tool.

**Tools:** Julia, Python, BoTorch, CUDA.
