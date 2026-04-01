# IDEC-MNIST-Clustering
An Improved Deep Embedded Clustering (IDEC) implementation applied to the MNIST dataset.

## Overview
This repository contains a PyTorch implementation of Improved Deep Embedded Clustering (IDEC) used to cluster the MNIST dataset in an unsupervised manner. 

IDEC improves upon standard Deep Embedded Clustering (DEC) by preserving the local structure of the data-generating distribution through the joint optimization of clustering label assignment and the autoencoder reconstruction loss.

## Features
- **Autoencoder Pretraining**: Learns a robust initial latent feature representation.
- **Joint Optimization**: Fine-tunes the network with both clustering loss (KL divergence) and reconstruction loss (MSE).
- **Evaluation Metrics**: Automatically calculates Unsupervised Clustering Accuracy (ACC), Normalized Mutual Information (NMI), and Adjusted Rand Index (ARI).
- **Visualizations**: Includes visualizations for data manifolds (t-SNE/UMAP), confusion matrices, and cluster purity distribution.

## Requirements
To run the notebook, install the following dependencies:
- Python 3.x
- PyTorch & Torchvision
- Scikit-learn
- NumPy & Pandas
- Matplotlib & Seaborn
- UMAP-learn (optional)

## Usage
1. Clone the repository.
2. Ensure you have the required dependencies installed.
3. Open and run all cells in `ptidec.ipynb`. The notebook will automatically download the MNIST dataset, train the autoencoder, perform IDEC, and save the resulting metrics and visualizations to the `results/` folder.
