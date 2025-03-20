# Project based on the paper "On Empirical Bayes Variational Autoencoder: An Excess Risk Bound"

## Objectives
This repository contains the implementation and experimental results related to Empirical Bayes Variational Autoencoders (EBVAEs), a generalization of traditional VAEs aimed at improving latent space representation by learning a more flexible prior distribution. Our work is inspired by the theoretical framework introduced by Tang and Yang (2021) and extends their findings through empirical evaluation.

## Goal
Our goal is to explore the theoretical and empirical advantages of **Empirical Bayes Variational Autoencoders (EBVAEs)** by analyzing their excess risk bounds and evaluating their performance in generating high-quality samples with optimized latent space representations.

## Features
- Implementation of **Empirical Bayes VAEs (EBVAEs)**
- Comparison with standard VAEs on the **MNIST** and **Fashion-MNIST** datasets
- Evaluation of excess risk bounds and empirical performance
- Analysis of the impact of optimizing the covariance matrix of the latent distribution

## Experiments
We test the effectiveness of **Empirical Bayes VAEs (EBVAEs)** by:
- Training EBVAEs and standard VAEs on MNIST and Fashion-MNIST datasets.
- Evaluating model performance based on **log-likelihood, FID scores**, and **sample quality**.
- Analyzing whether learning the full covariance matrix of the latent distribution improves generation quality.

## Results

## References
- Tang, R., & Yang, Y. (2021). *On Empirical Bayes Variational Autoencoder: An Excess Risk Bound*. **Conference on Learning Theory (COLT)**.

## Contributors
- **Elif Nebioglu** (ENS Paris Saclay)
- **Liam Ludington** (ENS Paris Saclay)


