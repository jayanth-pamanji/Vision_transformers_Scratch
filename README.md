# **Vision Transformer (ViT) from Scratch**

This project implements a **Vision Transformer (ViT)** model from scratch using PyTorch, demonstrating how self-attention and transformer blocks can be applied to image classification tasks. The notebook walks through every major component in a step-by-step educational manner.

---

## **📚 Overview**

The **Vision Transformer (ViT)** is a novel deep learning architecture that applies the principles of transformers—originally developed for natural language processing—to image data. Instead of processing the entire image as a grid of pixels or using convolutional filters, ViT divides an image into small fixed-size patches and processes them as a sequence of tokens.

Each image is:
- Split into **patches** (e.g., 4x4 pixels)
- Flattened and linearly projected into a fixed-dimension embedding
- Augmented with **position encodings** to retain spatial information
- Fed through a standard **transformer encoder** made up of self-attention and feedforward blocks
- A special **[CLS] token** is used for classification at the end

ViTs have shown competitive performance with convolutional neural networks (CNNs), especially when trained on large-scale datasets.

---

## **🧠 Model Architecture**

The architecture consists of the following components:

- **Patch Embedding Layer**: Converts 2D image patches into 1D vectors and projects them into an embedding space.
- **Positional Encoding**: Adds positional information to patch embeddings since transformers are order-agnostic.
- **Transformer Encoder Blocks**: Multiple layers of multi-head self-attention and feedforward neural networks.
- **Classification Token ([CLS])**: A learnable token prepended to the sequence for classification tasks.
- **MLP Head**: A final fully connected layer applied to the [CLS] token for classification output.

---

## **📊 Hyperparameters**

- `batch_size = 64`  
- `img_size = 28`  
- `patch_size = 7`  
- `num_channels = 1`  
- `num_patches = (img_size // patch_size) ** 2`  
- `num_heads = 1`  
- `embed_dim = 16`  
- `mlp_dim = 16`  
- `transformer_units = 1`
