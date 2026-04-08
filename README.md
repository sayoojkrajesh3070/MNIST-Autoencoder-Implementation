# MNIST Autoencoder Implementation

## Project Overview
This project involves building and training a basic **Autoencoder** using the **MNIST dataset** of handwritten digits.The goal is to implement an unsupervised learning model that compresses input images into a lower-dimensional latent space and subsequently reconstructs them.

## Model Architecture
The model is composed of two primary functional components:

*1.**Encoder**: Flattens the $28\times28$ grayscale image (784 pixels) and compresses it into a **32-unit latent representation** using Dense layers with ReLU activation.

*2.**Decoder**: Reconstructs the original image from the latent space using a series of Dense layers, ending with a **Sigmoid activation** to ensure output pixel values remain between 0 and 1.

### Model Summary
The following requirements were met for the architecture:
* **Input Shape**: $28 \times 28 \times 1$.
* **Latent Dimension**: 32 units.
* **Structure**: Symmetrical Encoder-Decoder design.

---

## Training and Evaluation
The autoencoder was trained on the **MNIST training dataset** and evaluated using the **test dataset**.
* **Optimizer**: Adam
* **Loss Function**: Mean Squared Error (MSE)
* **Epochs**: 10
* **Batch Size**: 256

### Performance Results
* **Loss Curves**: The training and validation loss curves show steady convergence, indicating that the model effectively learned the underlying features of the digits.
* **Reconstruction**: Side-by-side comparisons of the original test images versus the model's output demonstrate high-fidelity reconstruction where the identity of each digit is clearly preserved.

---

## Deliverables
As per the assignment requirements:
* **Model Architecture & Summary**: Implemented and displayed.
* **Training & Loss Curves**: Plotted for both training and validation sets.
* **Reconstruction Results**: Original vs. Reconstructed images displayed.
* **Code Quality & Explanation**: Well-structured code with a short results explanation.

---
