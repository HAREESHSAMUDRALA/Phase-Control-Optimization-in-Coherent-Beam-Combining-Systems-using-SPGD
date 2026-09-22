# Phase Control Optimization in Coherent Beam Combining (CBC) Systems using SPGD

**Author:** Samudrala Hareesh
**Guide:** Dr. Balaji Srinivasan, Professor, Department of Electrical Engineering, IIT Madras
**Date:** July 10, 2024

## Overview

This work compares multiple gradient-based optimization techniques for phase locking in Coherent Beam Combining (CBC) systems using Stochastic Parallel Gradient Descent (SPGD).

## Key Findings

- **Adam** — fast response to rapid phase changes, but less stable
- **AdaGrad** — struggles with phase locking due to aggressive learning rate decay
- **Adadelta** — improves on AdaGrad, but underperforms in highly dynamic conditions
- **RMSProp** — best overall balance of stability and agility for phase locking
- **AdaBelief** — strong generalization and stability, supports durable phase transitions
- **RAdam** — consistent performance via adaptive learning rate adjustment
- **AMSGrad** — improved reliability over Adam by resolving convergence issues, giving steady updates with low variance

## Conclusion

No single optimizer dominates across all conditions — the right choice depends on the trade-off between response speed and stability required for a given CBC setup. **RMSProp** emerges as the most balanced choice for phase locking, while **AMSGrad** and **AdaBelief** offer the most reliable convergence in dynamic environments.
