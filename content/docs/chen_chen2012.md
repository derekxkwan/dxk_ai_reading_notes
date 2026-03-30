---
title: "Extended BIC for small-n-large-P sparse GLM"
date: 2026-03-29T21:27:23-07:00
authors: ["Jiahua Chen", "Zehua Chen"]
year: 2012 
tags: ["bic", "bayesian", "information theory", "statistics"]
categories: ["statistics", "information theory"]
paper_url: ""
doi: "10.5705/ss.2010.216"
paper_src: ""
bibkey: "chen_chen2012"
math: true
draft: false
---

## Summary
Extends the BIC formulation with an additional term design to deal with situations with little data and a large number of parameters. Sets up mathematical formulation in the context of GLMs and also performs experiments using log-linear models.

Permissible values of new parameter $\gamma$ are between 0 and 1 with $0$ being equivalent to BIC. Shows benefits over BIC with $\gamma \ge 0.5$.

Defines consistency specifications where EBIC holds (A1-A6).

Defines false discovery rate (FDR) and positive selection rate (PSR). Consistency is proven for "normal linear models" ($FDR \rightarrow 0$ and $PSR \rightarrow 1$ as $n \rightarrow \infty$) and $\gamma$ values shown to "keep FDR low" and attain "a reasonable PSR". 

## Key Contributions
Extension of BIC to large parameter models (which BIC performs poorly in).

## Limitations and Future Work


## Key Equations
### GLM of interest here
- $f(y; \theta) = \exp(\theta^Ty - b(\theta)$
    - $E(Y) = b^{\prime}(\theta) = \mu$
    - $Var(Y) = b^{\prime \prime}(\theta) = \sigma^2)$
    - MGF: $M(t) = \exp(b(\theta+t) - b(\theta)$
### EBIC
- $EBIC(s) = -2l_n(\hat{\beta}(s)) + \nu(s) \log n + 2 \nu(s) \gamma \log P$
### Theorems (with Claude summaries)
- 1 (under A1-A6): $\max\limits_{s \in A_0} \lVert \hat{\beta}(s) - \beta_0(s) \rVert = O_p(n^{-\frac{1}{3}})$ as $n \rightarrow \infty$
    - $\hat{\beta}(s)$ MLE of $\beta(s)$ for GLM
    - MLE of any overfitted model converges to true parameters at given rate (usually $\sqrt{n}$)
- 2a (under A1- A6): $\mathbb{P}[\min\limits_{s \in A_1} EBIC(s) \le EBIC(s_0)] \rightarrow 0$ as $n \rightarrow \infty$ for $\gamma > 0$
    - EBIC never prefers an underfitted model over the true model for $\gamma > 0$
- 2b (under A1- A6): $\mathbb{P}[\min\limits_{s \in A_0, s \neq s_0} EBIC(s) \le EBIC(s_0)] \rightarrow 0$ as $n \rightarrow \infty$ for $\gamma > 1 - \frac{\log n}{2 \log P}$
    - EBIC never prefers an overfitted model over the true model for $\gamma > 1 - \frac{\log n}{2 \log P}$
    - both 2a and 2B hold for $Kn^{\kappa} = o(n^{\frac{1}{3}})$ ($K = O(\log n)$)
- 3 (under A1- A3, A4' A5', A6): $\mathbb{P}[EBIC(k) > EBIC(k+1)] \rightarrow 1$ as $n \rightarrow \infty$
    - $\theta_{0i} = \bm{x}_i^T \bm{\beta}_0$ 
    - $EBIC(k) = \min \{ EBIC(s): \nu(s) = k\}$ for any $\gamma > 0$ and $k < \nu(s_0)$
    - A4', A5' based on supremum of expectation of log likelihood (using $E[Y] = b^{\prime}$): $G_n(k) = \sup \{\sum\limits_{i=1}^n [\theta_i b^{\prime}(\theta_{0i}) - b)\theta_i)]: \theta_i = \bm{x}_i(s)^T \bm{\beta}(s); \nu(s) = k \}$
    - EBIC correctly orders models by size below the true sparsity (if $k < \nu(s_0)$, adding another feature improves EBIC).

### Metrics
- PSR: $\frac{\sum_{j=1}^N \nu(s_j^{*} \cup s_0)}{N \nu(s_0}$
- FDR = $\frac{1}{N} \sum\limits_{j=1}^N \frac{\nu(s_j^{*}/s_0}{v(s_j^{*})}$
- $s_j^{*}$: "features selected in $j$th replicate ($j = 1 \dots N$)
## Other Notes
 - Natural parameter space $\Theta = \{ \theta: \int \exp(\theta^T y) d \nu < \infty\}$ as well as $\eta$ are the range of the canonical link function $g$ so $g(\mu) = \eta = x^T \beta$ 
   
### Notation
- $y_i$: response variable (prediction)
- $x_i$: feature vector ($D$ dimensional)
- $s$: subset of $\{1 \dots D\}$
- $\nu(s)$: cardinality of $s$
- $\beta(s)$: parameter vector with dimensions corresponding to $s$ nonzero
- $s_0$: support of distribution
- $\nu(s_0)$: true sparsity
- $\beta_0 = \beta(s_0)$: true parameter vector
- $A_0$: all subsets $s$ that contain $s_0$ (overfitted models)
- $A_1$: all subsets $s$ that do not contain $s_0$ (underfitted models)

