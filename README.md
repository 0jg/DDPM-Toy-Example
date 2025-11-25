# DDPM-Toy-Example

A minimal working example of a Denoising Diffusion Probabilistic Model (DDPM) implemented in PyTorch.

## Overview

This repository contains a toy example demonstrating the core concepts of Denoising Diffusion Probabilistic Models (DDPMs), a class of generative models that learn to generate data by gradually denoising a normally distributed variable.

## What is DDPM?

Denoising Diffusion Probabilistic Models are a type of generative model that work by:

1. **Forward Process (Diffusion)**: Gradually adding Gaussian noise to data over a series of timesteps until the data becomes pure noise
2. **Reverse Process (Denoising)**: Learning to reverse the diffusion process by predicting and removing noise step by step, ultimately generating new samples from random noise

The model learns to estimate the noise added at each step, enabling it to generate new samples by starting from pure noise and iteratively denoising.

## Features

- Simple, educational implementation of DDPM
- PyTorch-based for easy understanding and modification
- Minimal dependencies for quick setup
- Well-commented code explaining key concepts

## Requirements

- Python 3.7+
- PyTorch
- NumPy
- Matplotlib (for visualization)

## Installation

```bash
git clone <repository-url>
cd DDPM-Toy-Example
pip install torch numpy matplotlib
```

## Usage

Run the notebook or script to see DDPM in action on a simple toy dataset. The example demonstrates:

- Setting up the noise schedule
- Implementing the forward diffusion process
- Training a simple neural network to predict noise
- Sampling new data points using the learned model

## References

- [Denoising Diffusion Probabilistic Models](https://arxiv.org/abs/2006.11239) - Ho et al., 2020
- [Understanding Diffusion Models: A Unified Perspective](https://arxiv.org/abs/2208.11970) - Luo, 2022

## License

This project is released into the public domain under the [Unlicense](LICENSE). See the LICENSE file for details.
