---
layout: single
title: "Course Project: CS860 Polynomial Auditing for Black-Box Differentially Private Mechanisms"
collection: projects
permalink: /projects/cs860-polynomial-auditing/
excerpt: "A course project on conservative black-box auditing of differential privacy through polynomial approximation of trade-off functions."
---

## Course Description
This course project studies differential privacy and privacy auditing from a theoretical and computational perspective. It focuses on how privacy guarantees can be evaluated in black-box settings, where the auditor observes only mechanism outputs rather than internal model parameters or training details.
---

## Course Project
In my [course project](https://kaixin-zheng.github.io/files/CS860_project_April_9.pdf), I studied black-box auditing of differential privacy by globally approximating the trade-off function. Instead of estimating privacy at isolated operating points, the project fits a conservative upper envelope to the observed trade-off curve and converts the fitted curve into an audited \((\varepsilon, \delta)\)-DP guarantee through tangent geometry.

The proposed method uses an even convex polynomial in rotated coordinates to enforce structural properties motivated by valid trade-off functions. I evaluated the approach on the Gaussian mechanism and a toy DP-SGD setting with analytic ground truth. The results show that polynomial fitting can recover reasonably tight estimates in clean settings and remains informative under noisy observations, while also revealing limitations such as tail sensitivity, noise in estimated trade-off pairs, and structural mismatch for asymmetric mechanisms.
