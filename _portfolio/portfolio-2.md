---
title: "Building a Vision Transformer from Scratch"
excerpt: "Saurabh P. Nale<br/><img src='/images/saurabh/vit/vit-portfolio.png'>"
collection: portfolio
---

# Project Overview:

Our project implements a Vision Transformer that classifies images from CIFAR-10, a dataset of 60,000 32x32 color images across 10 classes (e.g., cats, dogs, airplanes). The codebase is organized into modules for the model, data handling, training, and visualization, making it easy to extend or reuse. We’ll train the model using a train.py script and use a configuration file to manage hyperparameters. 

## Setting Up the Project

Let’s get started by setting up the environment.

1. **Clone the Repository**: Clone the project from GitHub to your local machine:

   ```bash
   git clone https://github.com/saurabhsensai/ViT-From-Scratch.git
   cd ViT-From-Scratch
   ```

2. **Install Dependencies**: The project uses PyTorch, torchvision, and other libraries listed in `requirements.txt`. Install them with:

   ```bash
   pip install -r requirements.txt
   ```

3. **Explore the Structure**: The repository is organized for clarity:

   - `vit/`: Contains modules for the model, dataset, trainer, and visualizer.
   - `scripts/`: Holds the training script (`train.py`).
   - `configs/`: Stores hyperparameters in `config.yaml`.
   - `README.md`: Provides setup and usage instructions.

## Understanding the Vision Transformer

Before diving into the code, let’s break down how a ViT works.

### Key Components

- **Patch Embedding**: The input image is split into fixed-size patches (e.g., 16x16 pixels). Each patch is flattened and projected into a vector, creating a sequence of embeddings.
- **Positional Embedding**: Since transformers don’t understand spatial order, we add positional embeddings to encode the location of each patch.
- **Attention Mechanism**: The transformer uses self-attention to weigh the importance of each patch relative to others, capturing global dependencies.
- **Transformer Blocks**: Multiple layers of attention and feed-forward networks process the patch sequence.
- **Classification Head**: A special “class token” aggregates information from all patches, and a linear layer outputs class probabilities.

## Code Walkthrough

Let’s explore the key components of the codebase without getting lost in the details. Each module is designed to be self-contained and reusable.

### 1. Model Architecture

- **Patch Embedding**: Converts image patches into vectors.
- **Attention**: Computes attention scores to focus on relevant patches.
- **Transformer Blocks**: Stack attention and MLP layers for deep processing.
- **Classification Head**: Maps the class token to output classes.

Key parameters like patch size and embedding dimension are configurable, allowing you to experiment with different setups.

### 2. Dataset Handling

The dataset module loads CIFAR-10 and applies transformations:

- **Training**: Resizes images to 224x224, applies random flips and rotations, and normalizes pixel values.
- **Validation**: Resizes and normalizes without augmentation.
- Data loaders batch the images for efficient training.

### 3. Training Logic

The training module handles the training loop:

- **Forward Pass**: Feeds images through the model.
- **Loss Calculation**: Uses cross-entropy loss.
- **Optimization**: Updates weights with AdamW and a cosine annealing scheduler.
- **Validation**: Evaluates performance on the test set and saves the best model.

### 4. Visualization Tools

Visualization is key to understanding ViTs. The visualizer module offers:

- **Patch Visualization**: Shows how images are divided into patches.
- **Embedding Visualization**: Uses t-SNE to plot patch or token embeddings, revealing class separation.
- **Attention Maps**: Displays which parts of the image the model focuses on, with overlays for clarity.

### 5. Configuration

Hyperparameters live in `config.yaml`, including:

- Image size (224x224).
- Batch size (16).
- Number of epochs (10).
- Learning rate (0.0003).
- Model specifics (e.g., 6 transformer layers, 12 attention heads).

Edit this file to tweak settings without touching the code.

<a href="https://github.com/saurabhsensai/ViT-From-Scratch" target="_blank">
  <img src="https://img.shields.io/badge/Open%20in-GitHub-black?logo=github" alt="Open in GitHub"/>
</a>
