# DeltaNet: Theory-Guided Autoregressive Policy Optimization for Optimal Dispatch of Heterogeneous Frequency Regulation Resources

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Pytorch](https://img.shields.io/badge/Pytorch-1.10%2B-red)](https://pytorch.org/)

This is the official implementation of the paper: **"DeltaNet: Theory-Guided Autoregressive Policy Optimization for Optimal Dispatch of Heterogeneous Frequency Regulation Resources"**.

> **Abstract:** > With the increasing penetration of renewable energy, coordinating heterogeneous Distributed Energy Resources (DERs) with conventional units is critical for secondary frequency regulation. This paper presents **DeltaNet**, a novel Autoregressive Factored MDP (AF-MDP) framework. Unlike monolithic agents, DeltaNet decomposes the joint dispatch policy into a conditional dependency chain. Crucially, we introduce a **Constraint Parameterization** mechanism that architecturally guarantees zero constraint violations without relying on reward penalties. Simulation results demonstrate that DeltaNet achieves superior regulation mileage and tracking precision while strictly adhering to physical limits.

## 🏗️ Architecture

![DeltaNet Framework](assets/framework.png)
*Fig. 1: Schematic of the DeltaNet architecture employing autoregressive sequential decision-making and constraint parameterization.*

## 🚀 Key Features
* **Physics-Constrained:** Guarantees safety (e.g., Ramp rates, SOC limits) via differentiable constraint parameterization.
* **Autoregressive Policy:** Decouples strong correlations among heterogeneous resources (Thermal, Hydro, LNG, BESS, EVs).
* **Theory-Guided Reward:** Optimizes a simplified $\ell_1$-norm objective proved to be asymptotically equivalent to the PJM performance score.

## 🛠️ Installation

1. Clone this repository:
   ```bash
   git clone [https://github.com/YourUsername/DeltaNet.git](https://github.com/YourUsername/DeltaNet.git)
   cd DeltaNet
