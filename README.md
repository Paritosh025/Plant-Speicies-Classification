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
```

---

## 📊 Outputs

- `val_accuracy_comparison.png` → model-wise validation accuracy chart  
- `val_loss_comparison.png` → model-wise validation loss chart  
- `*_results.pt` files generated during runs (saved metrics + checkpoint path)

---

## 🚀 How to Run

### Option A: Google Colab (recommended for current scripts)

The scripts are exported from Colab notebooks and already include:
- dependency install steps
- Kaggle API upload flow
- dataset download commands
- training + evaluation code

Run each file workflow in Colab to reproduce model training and comparison outputs.

### Option B: Local setup (manual adaptation)

```bash
pip install kaggle pytorch-lightning efficientnet_pytorch opencv-python-headless
```

Then adapt/remove Colab-specific commands (e.g., `files.upload()`, shell `!` commands) before running locally.

---

## 💼 Recruiter Highlights

- Practical deep learning implementation across **CNN + Transfer Learning + Transformer**
- Strong exposure to **computer vision experimentation**
- Hands-on with **model benchmarking and comparative analysis**
- Built using industry-relevant stack: **PyTorch, Lightning, torchvision, sklearn**

---

## 🔁 Suggested Next Improvements

- Add final metrics table directly in README
- Add inference script for single-image prediction
- Add confusion matrix and per-class performance visualization
- Refactor Colab-exported scripts into a clean modular package

---

## 📝 Note on Repository Name

The intended name is **Plant-Species-Classification**.  
If the current GitHub repository still shows `Plant-Speicies-Classification`, rename it from:

**GitHub Repo → Settings → Repository name**

---

If you’d like, I can also generate a **“final polished recruiter edition”** README with your name, project links, and top achievements formatted for portfolio impact.
