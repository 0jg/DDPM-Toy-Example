# DDPM-Toy-Example

A minimal working example of a Denoising Diffusion Probabilistic Model (DDPM) implemented in PyTorch.

## Overview

This repository contains examples demonstrating the core concepts of Denoising Diffusion Probabilistic Models (DDPMs), a class of generative models that learn to generate data by gradually denoising a normally distributed variable.

### Notebooks

1. **[ddpm_toy_example.ipynb](ddpm_toy_example.ipynb)** - A minimal 2D toy example with two Gaussian clusters. Great for understanding the core mathematics and visualizing the diffusion process.

2. **[ddpm_cifar10_cats.ipynb](ddpm_cifar10_cats.ipynb)** - DDPM applied to real images (cat images from CIFAR-10). Demonstrates how the same principles scale to 32×32 RGB images using a U-Net architecture.

## What is DDPM?

Denoising Diffusion Probabilistic Models are a type of generative model that work by:

1. **Forward Process (Diffusion)**: Gradually adding Gaussian noise to data over a series of timesteps until the data becomes pure noise
2. **Reverse Process (Denoising)**: Learning to reverse the diffusion process by predicting and removing noise step by step, ultimately generating new samples from random noise

The model learns to estimate the noise added at each step, enabling it to generate new samples by starting from pure noise and iteratively denoising.

## Usage

Run either notebook to see DDPM in action:

- **Toy Example**: Simple 2D demonstration on synthetic data
- **CIFAR-10 Cats**: Image generation on real cat images

Both examples demonstrate:

- Setting up the noise schedule
- Implementing the forward diffusion process
- Training a neural network to predict noise
- Sampling new data points using the learned model

## References

- [Denoising Diffusion Probabilistic Models](https://arxiv.org/abs/2006.11239) - Ho et al., 2020

## License

This project is released into the public domain under the [Unlicense](LICENSE). See the LICENSE file for details.
