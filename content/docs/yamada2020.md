---
title: "Feature Selection using Stochastic Gates"
date: 2026-02-07T22:51:43-08:00
authors: ["Yutaro Yamada", "Ofir Lindenbaum", "Sahand Negahban", "Yuval Kluger"]
year: 2020
tags: ["feature selection", "sparse", "bernoulli", "neural network", "reparamerization trick", "empirical risk minimization", "mutual information", "markov blanket"]
categories: ["supervised", "probabilistic"]
paper_url: "https://proceedings.mlr.press/v119/yamada20a.html"
doi: ""
paper_src: "Proceedings of the 37th International Conference on Machine Learning"
bibkey: "yamada2020"
math: true
draft: false
---

## Summary
Constructs a method of feature selection for neural networks using a Bernoulli vector variable defined as $z_d = \max(0, \min(0(1, \mu_d + \epsilon_d))$. Maximizes mutual info between $\bm{X}_{\mathcal{S}}$ and $Y$ such that $|\mathcal{S}| = k$ where $k$ is number of features as $\bm{X}_{\mathcal{S}}$ denotes the selected features of $\bm{X}$. Performs better than Hard-Concrete as it is high variance.

## Key Contributions
Relxation of Bernoulli variables using clipped Gaussians for feature selection and differentiating $L_0$ norm using reparameterization trick.

## Limitations and Future Work


## Key Equations
Empirical Risk: $\min_\limits{\theta,\mu} \hat{\mathbb{E}}_{X,Y} \mathbb{E}_Z [L(f_{\theta}(\bm{X} \odot \bm{Z}),Y) + \lambda \Vert \bm{Z} \Vert_0]$ 

Gradient of $\lambda \Vert \bm{Z} \Vert_0$: $\frac{1}{K}\sum\limits_{k=1}^K [L^{\prime}(\bm{z^{(k)}}) \frac{\partial z_d^{(k)}}{\partial \mu_d} ] + \lambda \frac{\partial}{\partial \mu_d} \Phi(\frac{\mu_d}{\sigma})$
## Other Notes
