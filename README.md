# Protein Expression Profile Prediction from Gene Expression Profile

This repository hosts the code for a Contractive Autoencoder model and a Variational Autoencoder model designed to perform multi-task learning on biological data, particularly for predicting mRNA expression profiles, protein expression profiles, and cancer types from RNA expression profiles.

## Overview

The model employs a Contractive Autoencoder  and a Variational Autoencoder architecture that encodes high-dimensional transcription profiles into a compact latent vector. The encoded representations are then used to reconstruct mRNA and protein expression profiles, as well as to classify disease type, making it a multi-task learning system. This architecture has been trained and validated on a dataset consisting of mRNA transcription profiles from 7150 clinical samples across 32 classes from The Cancer Genome Atlas (TCGA) dataset and The Cancer Proteome Atlas (TCPA) .

## Features

- **Contractive Autoencoder and Variational Autoencoder models**: Regularizes the learning process to learn a robust latent space.
- **Multi-Task Learning**: Simultaneously predicts multiple outputs - mRNA levels, protein levels, and disease type.
- **Gaussian Noise and Dropout**: Improves generalization by preventing overfitting.
- **Batch Normalization**: Accelerates training and provides regularization.
- **Custom Loss Function**: Combines mean squared error with a contractive penalty to enhance learning of the latent space.

## Requirements

To run this model, you will need the following:

- Python 3.x
- TensorFlow 2.x
- Keras

You can install the necessary libraries using pip:

```bash
pip install tensorflow
pip install keras
```

