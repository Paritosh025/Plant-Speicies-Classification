# 🌿 Plant-Species-Classification

> Deep learning benchmark project for **multi-class plant species recognition** using PyTorch Lightning and transfer learning.

![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-Deep%20Learning-red)
![PyTorch Lightning](https://img.shields.io/badge/Framework-PyTorch%20Lightning-purple)
![Status](https://img.shields.io/badge/Status-Active-success)

---

## 📌 Project Overview

This repository compares multiple modern vision architectures for classifying plant species from images (Kaggle **Plant Seedlings Classification** dataset).  
The goal is to build an end-to-end image classification workflow and evaluate which model family works best for this task.

### ✅ Models Implemented
- Custom **CNN**
- **ResNet18** (pretrained)
- **DenseNet121** (pretrained)
- **EfficientNet-B0** (pretrained)
- **ViT-B/16** (Vision Transformer, pretrained)

---

## 🔬 What This Project Demonstrates

- End-to-end dataset preparation and train/validation split
- Data augmentation with torchvision transforms
- Transfer learning + fine-tuning across multiple architectures
- Reproducible training loops using **PyTorch Lightning**
- Validation metric/loss comparison and visual reporting
- Saved model result artifacts (`*.pt`) for cross-model benchmarking

---

## 🧠 Training Workflow

1. Download dataset from Kaggle
2. Split dataset into train/val folders (class-wise)
3. Train each model independently
4. Validate and save:
   - best checkpoint path
   - validation accuracy
   - validation loss
5. Compare all models through generated plots

---

## 📁 Repository Structure

```text
Plant-Species-Classification/
├── cnn.py
├── resnet18.py
├── densenet121.py
├── efficientnet_b0.py
├── vit_b_16.py
├── val_accuracy_comparison.png
└── val_loss_comparison.png
