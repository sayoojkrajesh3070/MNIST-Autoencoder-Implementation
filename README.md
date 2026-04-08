# MNIST Autoencoder Implementation

## Project Overview
[cite_start]This project involves building and training a basic **Autoencoder** using the **MNIST dataset** of handwritten digits[cite: 1, 2]. [cite_start]The goal is to implement an unsupervised learning model that compresses input images into a lower-dimensional latent space and subsequently reconstructs them[cite: 4, 5].

## Model Architecture
[cite_start]The model is composed of two primary functional components[cite: 20]:

1.  [cite_start]**Encoder**: Flattens the $28\times28$ grayscale image (784 pixels) and compresses it into a **32-unit latent representation** using Dense layers with ReLU activation[cite: 4].
2.  [cite_start]**Decoder**: Reconstructs the original image from the latent space using a series of Dense layers, ending with a **Sigmoid activation** to ensure output pixel values remain between 0 and 1[cite: 5].

### Model Summary
[cite_start]The following requirements were met for the architecture[cite: 19, 21]:
* [cite_start]**Input Shape**: $28 \times 28 \times 1$[cite: 4].
* **Latent Dimension**: 32 units.
* [cite_start]**Structure**: Symmetrical Encoder-Decoder design[cite: 20].

---

## Training and Evaluation
[cite_start]The autoencoder was trained on the **MNIST training dataset** and evaluated using the **test dataset**[cite: 7, 8].

* **Optimizer**: Adam
* **Loss Function**: Mean Squared Error (MSE)
* **Epochs**: 10
* **Batch Size**: 256

### Performance Results
* [cite_start]**Loss Curves**: The training and validation loss curves show steady convergence, indicating that the model effectively learned the underlying features of the digits[cite: 11, 25].
* [cite_start]**Reconstruction**: Side-by-side comparisons of the original test images versus the model's output demonstrate high-fidelity reconstruction where the identity of each digit is clearly preserved[cite: 12, 16, 27].

---

## Deliverables
[cite_start]As per the assignment requirements (Total = 10 marks)[cite: 13, 18]:
* [cite_start]**Model Architecture & Summary**: Implemented and displayed (2 marks)[cite: 19].
* [cite_start]**Training & Loss Curves**: Plotted for both training and validation sets (3 marks)[cite: 22].
* [cite_start]**Reconstruction Results**: Original vs. Reconstructed images displayed (3 marks)[cite: 26].
* [cite_start]**Code Quality & Explanation**: Well-structured code with a short results explanation (2 marks)[cite: 29, 31].

---

## How to Run
1. Ensure you have `tensorflow`, `numpy`, and `matplotlib` installed.
2. Open the `Autoencoder_Implementation.ipynb` file.
3. [cite_start]Run all cells to view the model summary, loss plots, and reconstruction results[cite: 10, 11, 12].
