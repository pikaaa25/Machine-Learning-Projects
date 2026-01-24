# Interpretable CNN for CIFAR-10 Image Classification

## Overview

This project focuses on building an **interpretable Convolutional Neural Network (CNN)** for **CIFAR-10 image classification**. In addition to achieving competitive accuracy, the model is designed to provide **human-understandable explanations** for its predictions using post-hoc and intrinsic interpretability techniques.

The goal is to improve **trust, transparency, and reliability** of CNN-based image classifiers by visualizing *what* the model learns and *why* it makes certain decisions.

## Dataset: CIFAR-10

* 60,000 color images (32×32)
* 10 classes: airplane, automobile, bird, cat, deer, dog, frog, horse, ship, truck
* 50,000 training images, 10,000 test images

## Model Architecture

A lightweight and interpretable CNN architecture:

* Convolutional layers with small kernels (3×3)
* Batch Normalization
* ReLU activations
* Global Average Pooling (GAP) instead of fully connected layers
* Softmax output layer

**Why GAP?**
Global Average Pooling preserves spatial correspondence and enables **Class Activation Maps (CAMs)**, improving interpretability.

## Interpretability Techniques Used

### 1. Class Activation Maps (CAM)

* Highlights image regions most influential for a class prediction
* Requires GAP-based CNN architecture

### 2. Grad-CAM

* Gradient-based localization technique
* Works with any CNN architecture
* Produces heatmaps showing important regions

### 3. Saliency Maps

* Uses input gradients to visualize pixel importance
* Simple but effective for local explanations

### 4. Feature Map Visualization

* Visualizes intermediate convolutional filters
* Helps understand learned low-level and high-level features

## Repository Structure

```
.
├── data/                 # CIFAR-10 dataset loaders
├── models/               # CNN architectures
├── training/             # Training scripts
├── explainability/       # CAM, Grad-CAM, saliency methods
├── evaluation/           # Accuracy and interpretability metrics
├── experiments/          # Reproducible experiments
├── results/              # Plots and heatmaps
├── configs/              # Configuration files
└── README.md
```

## Training

```bash
python training/train.py --dataset cifar10 --model interpretable_cnn
```

## Generating Explanations

```bash
python explainability/gradcam.py --image sample.png --class_id 3
```

## Evaluation Metrics

### Classification Performance

* Accuracy
* Precision / Recall
* Confusion Matrix

### Interpretability Evaluation

* Localization quality of heatmaps
* Visual coherence with object regions
* Qualitative human inspection

## Results (Typical)

* Test Accuracy: ~80–85% (lightweight CNN)
* Grad-CAM heatmaps align well with object regions
* Improved transparency compared to standard CNNs

## Applications

* Educational demonstrations of CNN behavior
* Safety-critical vision systems
* Model debugging and bias detection
* Trustworthy AI research

## Limitations

* Interpretability methods are approximate, not causal
* Heatmaps may vary with architecture and hyperparameters
* Human evaluation is subjective

## Future Work

* Concept-based explanations (TCAV)
* Prototype-based networks (ProtoPNet)
* Quantitative interpretability benchmarks
* Extension to OOD detection and uncertainty estimation



---

**Keywords:** Interpretable CNN, CIFAR-10, Explainable AI (XAI), Grad-CAM, CAM, Saliency Maps

