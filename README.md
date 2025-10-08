# Generative Digits with a Variational Autoencoder (VAE)

[![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)](https://keras.io/)

A deep learning notebook focused on building and training a **Variational Autoencoder (VAE)** with Keras on the MNIST dataset to generate new, original handwritten digits.

---

## 📖 Lab Overview

Variational Autoencoders are a fascinating type of **generative model** in deep learning. By learning the underlying latent representations of a dataset, they gain the ability to create entirely new data. VAEs can be used to draw faces, produce music, and, as we'll see in this lab, generate images of handwritten digits. ✍️

In this exercise, we will:
* Study the unique architecture of a VAE.
* Build a VAE from scratch using Keras and TensorFlow.
* Train our model on the MNIST digits dataset.
* Use the trained model to generate novel digit images that have never been seen before.



---

## 🔬 Core Concepts of VAEs

* **Generative Model:** Unlike discriminative models that predict labels, a generative model learns the distribution of the input data so it can create new samples from that distribution.
* **Probabilistic Latent Space:** The VAE encodes inputs into a latent space defined by a probability distribution (typically a Gaussian with a mean and variance). This smooth, continuous space allows us to sample points and decode them into realistic outputs.
* **Encoder-Decoder Architecture:**
    * The **Encoder** network takes an input image and outputs the parameters (mean and log-variance) of a distribution in the latent space.
    * The **Decoder** network takes a point sampled from the latent space and reconstructs it back into a full image.
* **The Reparameterization Trick:** A clever mathematical technique used to allow the gradient to flow through the random sampling process, making the entire network trainable with backpropagation.

---

## 🎯 Learning Objectives

By the end of this lab, you will be able to:

1.  Understand the key components that differentiate a VAE from a standard autoencoder.
2.  Implement the encoder, decoder, and sampling layers of a VAE in Keras.
3.  Define and use a custom loss function that includes both a reconstruction loss and a Kullback–Leibler (KL) divergence loss.
4.  Train a VAE on the MNIST dataset.
5.  Generate new images by sampling points from the learned latent space and passing them through the decoder.

---

