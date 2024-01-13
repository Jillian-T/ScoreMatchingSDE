# Diffusion Probabilistic Generative Models using Diffusion Bridge
## Introduction
The goal is to devlop a diffusion generative model via simulating diffusion bridge.

More specifically, we build a new generative model by establishing a Schrodinger Bridge between data samples and an easily-sampled noise distribution.

Via score-matching technique, the score function of the generative process can be estimated from the diffusion bridge between observations and latent variables.

The generative process can be described with a stochastic differential equation(SDE), that is why we name our project __ScoreMatchingSDE__

In __MNIST_GEN.ipynb__, we build a diffusion pipeline to establish the diffusion bridge between MNIST data and gaussian noise (easily-sampled). Then we train a Unet model to match the score function of this process

This notebook can run in colab T4 runtime directly

## Requirements
* pytorch >= 1.8
* diffusers >= 0.21.4
* datasets >= 2.14.4
* imageio >= 2.31.1
