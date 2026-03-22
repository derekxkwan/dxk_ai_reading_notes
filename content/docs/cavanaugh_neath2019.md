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
This paper gives intuitions on using the AIC and what it estimates.

Given parameter space $\Theta(k)$ with elements $\theta_k$ and KL divergence between true model $g(y)$ and candidate model $f(y|\theta_k)$ $KL(\theta_k) = \mathbb{E}[\log \frac{g(y)}{f(y|\theta_k)}]$, we define Kullback discrepancy $d(\theta_k) = \mathbb{E}[-2 \log f(y | \theta_k)$ and note that $2 KL(\theta_k) = d(\theta_k) - \mathbb{E}[-2 \log g(y)]$. Since the second term is the same given all candidate models, we drop it and judge candidate models by Kullback disprepancy.

We can define $AIC = -2 \log f(y| \hat{\theta}_k) + 2k$ and note that asymptotically approaches the expected value of $\Delta(k) = \mathbb{E}[d(\hat{\theta}_k]$ where expectation is taken first over $y$ then $\theta_k$.

AIC is noted to be **asymptotically efficient** (find models that are "predictively optimal" asymptotically even if true model not in parameter space) and **not consistent** (will not select correct model/structure, which BIC will do). AIC is noted to be **predictive** (predict new data) rather than **descriptive** (ID important factors in output, BIC).

AIC and BIC are then viewed in the predictive lens using a validation data $z$.

Extensions of AIC are discussed ($AIC_c$, $TIC$) and AIC is compared to $R^2_{adj}$ and Mallows $C_p$. A table is presented where all criterion are said to take the form $-2 log f(y | \hat{\theta}) + a_n k)$ where $R^2_adj$ has form $a_n k = k$, AIC/TIC/$C_p$/PRESS have form $2k$ (predictive), CAIC has form $k \log n + k$ (descriptive), and BIC form $k \log n$ (descriptive).
 
## Key Contributions
Overview of intuitions of AIC and comparison with BIC as well as other information criterion.

## Limitations and Future Work


## Key Equations
Kullback discrepancy: $d(\theta_k) = \mathbb{E}[-2 \log f(y | \theta_k)$

AIC: $-2 \log f(y|\hat{\theta}_k) + 2k$

$\Delta(k) = \mathbb{E}[d(\hat{\theta}_k)]$

$\Delta(k) = \mathbb{E}[ -2 log f(y | \hat{theta}] + (\mathbb{E}[-2 \log f(y | \theta_o] - \mathbb{E}[ -2 \log f(y | \hat{\theta}]) + ( \mathbb{E}[d(\hat{\theta})] - E[-2 \log f(y| \theta_o)])$ for true parameter vector $\theta_o$

## Other Notes
- both in-sample error and out-of-sample error $= k + o(1)$
- So $\Delta(k) = \mathbb{E}{d(\hat{\theta}_k)} = \mathbb{E}(-2 \log f(y | \hat{\theta}) + in-sample + out-of-sample = \mathbb{E}(-2 \log f(y | \hat{\theta}) + 2k$  
- Bootstrap sampling samples from a data distribution to get $\hat{\theta}^{*}$ and then validates on the full distribution (chance of non-selection of datapoint is $\frac{1 - \frac{1}{n}}{n}$ which goes to $\frac{1}{e}$ as $n \rightarrow \infty$
- For TIC, penalty term is $2 tr[J(\hat{\theta})[I(\hat{\theta})]^{-1}]$ where $J(\theta) = \mathbb{E}[(\frac{\partial \log f(y | \theta)}{\partial \theta})(\frac{\partial \log f(y | \theta)}{\partial \theta})^T]$
    - Note that variance of the score function = $\mathbb{E}[score \cdot score^T] - \mathbb{E}[score]\mathbb{E}[score]^T$ and at $\hat{\theta}$, $\mathbb{E}[score] = 0$ so we have $J{\theta}$
    - since $J(\hat{\theta}) = I(\hat{\theta})$, the expression is $2 Tr(I) = 2k$
- MSE refers to the unbiased estimator of $\sigma^2$ (variance of error) $\frac{SSE}{n-p}$ where $p$ is rank of design matrix and $SSE$ is sum of squared error so when $p$ increases, denominator decreases so MSE decreases
    - $\mathbb{E}[MSE] > \sigma_0^2$ for underspecified models, $=$ otherwise.
- Mallows $C_p = \frac{SSE}{MSE_{+}} - n + 2p$ where $MSE_+$ MSE of largest fitted model ($\mathbb{E}[MSE_{+}] = \sigma^2_0$)
    - correctly/overspecified $C_p approx p$, else $C_p > p$
### Notation
- Notation does not specify what expectations are over. Assume everything not fixed ($\hat{\theta}_k$ is an RV) is taken over the expectation.
### Intuition on Terms
- $\mathbb{E}[d(\hat{\theta})]$ is average performance of a model over different experiments (take $\mathbb{E}_y$ first and then take $\mathbb{E}_{\hat{\theta}}$)
- $\mathbb{E}[-2 \log f(y | \hat{\theta})]$ does the expectation over $y, \hat{\theta}$ at the same time ($y$ used to find $\hat{\theta}$) so it is training performance ($y$ is a single data point, $\hat{\theta}$ was found from $n_{train}$ points)
- $\mathbb{E}[-2 \log f(y | \theta_o)]$ does the expectation over $y$ ($\theta_o$ is the "true parameter vector"). We can count $f(y | \theta_o)$ as the true probability of an event so $y$ is the average probability of an event.
- $\mathbb{E}[-2 \log f(y | \theta_o)] - \mathbb{E}[-2 \log (f | \hat{\theta})]$ is in-sample estimation error. How far are off from the true probability of an event in-sample.
- $d(\hat{\theta}) - \mathbb{E}[-2 \log f(y | \theta_o)]$ is out-of-sample estimation error. How far are off from the true probability of an event out-of-sample (generalization error)
- Expected Fisher Information Matrix  $I(\theta) = \mathbb{E}[- \frac{\partial^2 \log f(y | \theta)}{\partial \theta \partial \theta^{\prime}}]$ takes the expectation over $y$ (take Hessian, average over $y$)
- Mean prediction error for future data $z$: $\Delta(k) = \mathbb{E} { -2 \log f (z | \hat{\theta}_k)$ where $\hat{\theta}_k$ arises from fitting to $y$ and the new expectation is over $z$.

