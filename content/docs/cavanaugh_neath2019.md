---
title: "The Akaike information criterion: Background, derivation, properties, application, interpretation, and refinements"
date: 2026-03-19T12:25:28-07:00
authors: ["Joseph E. Cavanaugh", "Andrew A. Neath"]
year: 2019
tags: ["statistics", "information theory", "aic", "frequentist"]
categories: ["statistics"]
paper_url: ""
doi: "10.1002/wics.1460"
paper_src: ""
bibkey: "cavanaugh_neath2019"
math: true
draft: false
---

## Summary


## Key Contributions


## Limitations and Future Work


## Key Equations


## Other Notes
- both in-sample error and out-of-sample error $= k + o(1)$
- So $\Delta(k) = \mathbb{E}{d(\hat{\theta}_k)} = \mathbb{E}(-2 \log f(y | \hat{\theta}) + in-sample + out-of-sample = \mathbb{E}(-2 \log f(y | \hat{\theta}) + 2k$  
### Notation
- Notation does not specify what expectations are over. Assume everything not fixed ($\hat{\theta}_k$ is an RV) is taken over the expectation.
### Intuition on Terms
- $\mathbb{E}[d(\hat{\theta})]$ is average performance of a model over different experiments (take $\mathbb{E}_y$ first and then take $\mathbb{E}_{\hat{\theta}}$)
- $\mathbb{E}[-2 \log f(y | \hat{\theta})]$ does the expectation over $y, \hat{\theta}$ at the same time ($y$ used to find $\hat{\theta}$) so it is training performance ($y$ is a single data point, $\hat{\theta}$ was found from $n_{train}$ points)
- $\mathbb{E}[-2 \log f(y | \theta_o)]$ does the expectation over $y$ ($\theta_o$ is the "true parameter vector"). We can count $f(y | \theta_o)$ as the true probability of an event so $y$ is the average probability of an event.
- $\mathbb{E}[-2 \log f(y | \theta_o)] - \mathbb{E}[-2 \log (f | \hat{\theta})]$ is in-sample estimation error. How far are off from the true probability of an event in-sample.
- $d(\hat{\theta}) - \mathbb{E}[-2 \log f(y | \theta_o)]$ is out-of-sample estimation error. How far are off from the true probability of an event out-of-sample (generalization error)
- Expected Fisher Information Matrix  $I(\theta) = \mathbb{E}[- \frac{\partial^2 \log f(y | \theta)}{\partial \theta \partial \theta^{\prime}}]$ takes the expectation over $y$ (take Hessian, average over $y$)
- Mean prediction error for future data $z$: $\Delta(k) = \mathbb{E} E { -2 log f (z | \hat{\theta}_k)$ where $\hat{\theta}_k$ arises from fitting to $y$ and the new expectation is over $z$.
- For TIC, penalty term is $2 tr[J(\hat{\theta})[I(\hat{\theta})]^{-1}]$ where $J(\theta) = \mathbb{E}[(\frac{\partial \log f(y | \theta)}{\partial \theta})(\frac{\partial \log f(y | \theta)}{\partial \theta})^T]$
    - Note that variance of the score function = $\mathbb{E}[score \cdot score^T] - \mathbb{E}[score]\mathbb{E}[score]^T$ and at $\hat{\theta}$, $\mathbb{E}[score] = 0$ so we have $J{\theta}$
    - since $J(\hat{\theta}) = I(\hat{\theta})$, the expression is $2 Tr(I) = 2k$
