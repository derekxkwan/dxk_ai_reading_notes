---
title: "The Bayesian information criterion: background, derivation, and applications"
date: 2026-03-15T22:13:13-07:00
authors: ["Andrew A. Neath", "Joseph E. Cavanaugh"]
year: 2012
tags: ["statistics", "information theory", "bic"]
categories: ["statistics"]
paper_url: ""
doi: "10.1002/wics.199"
paper_src: ""
bibkey: "neath_cavanaugh2012"
math: true
draft: false
---

## Summary
Derives a Bayesian Information Criterion for one model through second-order Taylor serior expansion of an integral for the posterior probability of a model $M_k$ (abbrev. $k$), taken around $\hat{\theta}_k$ (parameters maximizing likelihood $L(\theta_k | y) = f(y | \theta_k)$ over parameter space $\Theta(k)$ where the components are independent). Derivation results in log probabilities of prior of model $\pi(k)$ and log of fisher information $\tilde{\mathcal{I}}(\hat{\theta}_k, y)$ since they are bounded as sample size $n \arrow \infty$. 

States that Bayes factor (ratio of posteriors divided by priors) between two models can be apprixmated by $B_{12} = \exp(-\frac{1}{2} \Delta_{12})$ where $\Delta_{12} = BIC(k_1) - BIC(k_2)$.

Also states posterior probabilities $P(k|y)$ can be recovered through comparison to a model with minimum BIC value $k_{\blacklozenge}$.

Also gives a way to do model averaging $h(\delta | y)$ (like bagging) given a parameter of data $\delta$
## Key Contributions


## Limitations and Future Work


## Key Equations

Approximation of negative log posterior of model $k$ $-2 ln P(k | y)$

$-2 \ln P(k|y) \approx S(k|y) \approx -2 L(\hat{\theta}_k | y) + k ln(n)$ where $L(\hat{\theta}_k | y) = f(y | \hat{\theta_k})$ (likelihood)

Bayes factor approximation: 

$B_{12} = \exp(-\frac{1}{2} \Delta_{12})$ where $\Delta_{12} = BIC(k_1) - BIC(k_2)$.

Approximation of posterior probability:

$P(k|y) \approx \frac{\exp(-\frac{1}{2}\Delta_k}{\sum_{l=1}^L \exp{-\frac{1}{2} \Delta_l}}$ where $\Delta_k = BIC(k) - BIC(k_{\blacklozenge})$.

Model averaging:

$h(\delta| y) = \sum\limits_{l=1}^L h(\delta | k_l, y)P(k_l | y)$
## Other Notes
