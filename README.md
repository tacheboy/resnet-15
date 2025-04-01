# ResNet-15 for Electron and Proton Classification

## Overview
This repository contains a ResNet-15-like model designed for classifying single electron and proton data stored in `.hdf5` format. The model has been optimized to achieve high accuracy while minimizing overfitting.

## Running the Model
The model training and validation can be executed by running the provided Jupyter Notebook.

## Best Model
- **Model File:** `resnet15_15.pth`
- **Training Accuracy:** 77.90%
- **Validation Accuracy:** 74.72%

## Training Recommendations
- **Epochs:** 20 to 30 (Increasing epochs may boost accuracy up to ~80% before overfitting)
- **Optimizers:** AdamW (Recommended) or Adam
- **Best Hyperparameters:**
  - **Optimizer:** AdamW
  - **Learning Rate:** `5e-4`
  - **Weight Decay:** `1e-4`
  - **Scheduler:** `optim.lr_scheduler.CosineAnnealingLR(optimizer, T_max=4)`

## Usage
1. Load the notebook and execute all cells.
2. Train the model using the recommended settings.
3. Evaluate performance on validation data.

## Notes
- Further tuning of hyperparameters may improve accuracy.
- Care should be taken to avoid overfitting beyond ~80% accuracy.

## Acknowledgment
This project is developed for studying electron and proton classification using deep learning.