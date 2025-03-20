# Empirical Bayes Variational Autoencoders: Excess Risk Bound

## Overview
This repository contains code and experiments related to **Empirical Bayes Variational Autoencoders (EBVAEs)**, an extension of conventional VAEs that optimizes the **latent prior’s covariance matrix** to enhance sample quality and reconstruction. Our work is based on the theoretical framework established by **Tang and Yang (2021)**, which provides **excess risk bounds** for EBVAEs, offering insights into their statistical guarantees.

## Objectives
We aim to **validate the theoretical and empirical advantages** of EBVAEs by:
- Implementing **Empirical Bayes Variational Autoencoders (EBVAEs)**
- Comparing them with **standard VAEs** using the **MNIST** dataset
- Analyzing the **impact of learning a full covariance matrix** in the latent space


## Experiments
We test the effectiveness of EBVAEs through:
- Training **four different models** on MNIST:
  1. **Standard VAE**
  2. **VAE with learned covariance matrix**
  3. **VAE with learned noise parameter**
  4. **VAE with both learned covariance and noise parameter**
- Evaluating performance in terms of:
  - **Reconstruction loss**
  - **KL divergence**
  - **EBVAE loss**
  - **Generated sample quality**
- **Investigating whether a more expressive latent prior** improves generative quality

## Results
Our findings suggest:
- **Learning the covariance matrix** slightly improves KL divergence but may **deregularize the latent space**
- **Learning the noise parameter** enhances **reconstruction loss** and **EBVAE loss**
- **Joint optimization of covariance and noise** requires careful balancing to avoid unstable training
- The standard VAE **still outperforms** in terms of generated sample **diversity and accuracy**


## References
- Tang, R., & Yang, Y. (2021). *On Empirical Bayes Variational Autoencoder: An Excess Risk Bound*. **Conference on Learning Theory (COLT)**.
- Grünwald, P. D., & Mehta, N. A. (2020). *Fast rates for general unbounded loss functions: From ERM to generalized Bayes*. **Journal of Machine Learning Research**.
- Bartlett, P. L., Bousquet, O., & Mendelson, S. (2005). *Local Rademacher complexities*.

## Contributors
- **Liam Ludington** (ENS Paris-Saclay)
- **Elif Nebioglu** (ENS Paris-Saclay)
