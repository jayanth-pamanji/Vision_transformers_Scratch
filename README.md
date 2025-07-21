# Vision Transformer (ViT) from Scratch

This project implements a **Vision Transformer (ViT)** model from scratch using PyTorch, demonstrating how self-attention and transformer blocks can be applied to image classification tasks. The notebook walks through every major component in a step-by-step educational manner.

---

## 📚 Overview

The Vision Transformer applies the standard Transformer architecture directly to images by treating image patches as tokens, similar to words in NLP. This project aims to:

* Provide a clear understanding of ViT internals
* Implement the ViT architecture from scratch
* Train and evaluate the model on a sample dataset (e.g., CIFAR-10 or MNIST)

---

## 🧠 Model Architecture

* **Patch Embedding Layer**
* **Positional Encoding**
* **Multi-Head Self-Attention**
* **Feedforward (MLP) Block**
* **Transformer Encoder**
* **Classification Head**

---

## 📊 Hyperparameters

* **Image Size:** 32x32
* **Patch Size:** 4x4
* **Number of Patches:** 64
* **Embedding Dimension:** 128
* **Number of Transformer Layers:** 6
* **Number of Attention Heads:** 4
* **MLP Hidden Dimension:** 256
* **Dropout Rate:** 0.1
* **Learning Rate:** 3e-4
* **Batch Size:** 64
* **Epochs:** 30

---


## 🧪 Training and Evaluation

* **Dataset:** CIFAR-10 (can be changed)
* **Epochs:** 10–50
* **Optimizer:** Adam
* **Loss Function:** CrossEntropyLoss
* **Accuracy Achieved:** \~70–90% depending on hyperparameters
`
