# simple-mamba
This repository contains a simple PyTorch implementation of the **Mamba** architecture for image classification on the **CIFAR-10** dataset. Mamba is a state space model (SSM) designed to model long-range dependencies efficiently — offering an alternative to Transformers in sequence-based vision tasks.
It includes training a model from scratch for image classification tasks.

## 📌 Features

- ✅ Trainable Mamba-based classifier for CIFAR-10
- ✅ Clean and minimal PyTorch code
- ✅ Supports training from scratch
- ✅ Easily extendable to other vision tasks or datasets


## 🧠 What is Mamba?

[Mamba](https://arxiv.org/abs/2312.00752) is a Selective State Space Model introduced by Gu et al. (2023) for efficient sequence modeling. Unlike Transformers, Mamba avoids attention by using dynamic linear state-space operators with selective memory updates — enabling faster and scalable training, even in causal or streaming settings.

---

## 🗂️ Repository Structure

```bash
📦 Mamba-CIFAR
 ┣ 📄 mamba_image_classifier.py     # Main training script
 ┣ 📄 README.md                     # This file
```


## 🚀 Getting Started

### 1. Install necessary dependencies:

This project requires Python ≥ 3.8 and PyTorch ≥ 1.12.

Install all required dependencies using:

```bash
pip install torch torchvision
pip install mamba-ssm causal-conv1d

If you encounter PyTorch version or compiler issues (e.g., during building mamba-ssm), use the following safer option:
```bash
pip install mamba-ssm causal-conv1d --no-build-isolation


### To Clone the Repository

```bash
git clone https://github.com/yourusername/mamba-cifar10.git
cd mamba-cifar10

### Run the .ipynb file to train and test the model.

### Trained model is also uploaded in the repository.
```bash
mamba_cifar.pth
