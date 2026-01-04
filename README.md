# LANR-GNN
Official implementation for LANR-GNN paper
# LANR-GNN: Label-Aware Neighborhood-Resampling Graph Neural Network

This repository contains the official implementation of **LANR-GNN**, a Label-Aware Neighborhood-Resampling Graph Neural Network designed to address class imbalance in graph learning.

> We will continuously maintain and update this repository to ensure reproducibility and clarity of usage.

---

## ✨ Overview

LANR-GNN introduces a label-aware neighborhood resampling strategy that enlarges decision margins for minority classes while preserving global structure information. The framework is general and can be applied to various GNN architectures.

---

## 🛠 Environment & Dependencies

All experiments were implemented in **PyTorch 2.4.0 (Python 3.8)** on:

- 12-core CPU  
- NVIDIA RTX 4090 GPU (24GB VRAM)  
- 60GB RAM  

### Required packages

numpy                     1.24.3  
pyg                       2.6.1           
pyg-lib                   0.4.0  
pytorch                   2.4.0  
scikit-learn              1.3.0  
scipy                     1.9.3  
torch-cluster             1.6.3  
torch-scatter             2.1.2  
torch-sparse              0.6.18  
torch-spline-conv         1.2.2  
tqdm                      4.66.5   

---

## ⚙️ Training Configuration

LANR-GNN was optimized using:

- Optimizer: **Adam**
- Learning rate: **0.005**
- Epochs: **400 (full-batch)**
- Hidden dimension: **16**
- Aggregation: **1-hop neighbors**
- Neighbor sampling: **10**

Resampling hyperparameters:

- \( P^- = 0.5 \)
- \( P^+ = 0.7 \)

Baselines were tuned either using:
1. Their optimal parameters, or  
2. Hyperparameters reported in original papers.

## 🚀 Usage

We are organizing the code and usage instructions.

A detailed usage guide (including training, evaluation, and scripts) will be released soon.

## Data Availability

The datasets used in this study are available **on request** from the authors. 
The data are not publicly available due to confidentiality restrictions.
