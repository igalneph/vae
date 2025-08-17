# Variational Autoencoder & Supervised Classification on MNIST

---

## Access to Source Code

For academic integrity reasons, the full source code of this project is kept in a **private repository**.  
If you are a recruiter, hiring manager, or collaborator and would like to review the code,  
please feel free to [contact me](mailto:ygalnep@gmail.com).  
I will be glad to provide access upon request.

---

## Overview

![](https://i.imgur.com/QvdWJfM.png)

This project was completed as part of the **Advanced Course in Machine Learning**. It consists of two main parts:

1. **Supervised Classification** – Implementing and training a CNN classifier on the MNIST dataset using PyTorch.
2. **Variational Autoencoder (VAE)** – Implementing and training both amortized and latent-optimized VAEs on MNIST, analyzing reconstruction quality, sampling, and log-likelihood estimation.

The project was an exercise in deep learning model implementation, probabilistic modeling, and generative models.

---

## Part 1: Supervised Classification

* Implemented a **Convolutional Neural Network (CNN)** classifier on MNIST.
* Trained on a **subset of 20,000 images** (2,000 per digit class).
* Achieved **97%+ accuracy** on the test set.
* Loss and accuracy curves across epochs were analyzed.
* Experiments confirmed PyTorch's automatic differentiation and computational graph capabilities.

---

## Part 2: Variational Autoencoder (VAE)

* Implemented a **VAE with Gaussian latent variables** and trained it on MNIST.
* Explored two optimization strategies:

  * **Amortized Inference**: Encoder network outputs mean and variance for latent distribution.
  * **Latent Optimization**: Directly optimizing per-sample latent vectors.
* Applied the **reparameterization trick** for stable gradient flow.
* Used **ELBO (Evidence Lower Bound)** as the training objective.
* Conducted experiments:

  * Reconstruction quality across epochs.
  * Sampling from prior and comparing generations.
  * Ablation between amortized and latent optimization approaches.
  * Computing log-likelihoods of digits using Monte Carlo estimation.

---

## Key Findings

* Amortized inference produced smoother latent representations but sometimes overfitted reconstructions.
* Latent optimization gave sharper reconstructions but required careful initialization.
* Training curves aligned with theoretical expectations of VAE optimization.
* Certain digits (e.g., '1' and '7') were assigned higher log-likelihoods compared to others.

---

## Technologies & Tools

* **PyTorch** – Deep learning framework for model implementation.
* **Torchvision** – Dataset utilities and transforms.
* **Matplotlib / Plotly** – Visualization of training curves and results.
* **NumPy / SciPy** – Numerical operations.

---

## Author

**Yigal Nepomniachi**
