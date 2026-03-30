---
title: "Information criteria for model selection"
date: 2026-03-23T00:30:58-07:00
authors: ["Jiawei Zhang", "Yuhong Yang", "Jie Ding"]
year: 2023
tags: ["aic", "bic", "information criterion", "information theory", "statistics", "computational statistics"]
categories: ["statistics", "information theory"]
paper_url: ""
doi: "10.1002/wics.1607"
paper_src: ""
bibkey: "zhangyangding2023"
math: true
draft: false
---

## Summary
(partially read)

## Key Contributions


## Limitations and Future Work


## Key Equations
- consistency for $m_{*} = \arg \min_{m \in \mathbb{M}_w} d_m$ where $\mathbb{M}_w \triangleq \{ m \in \mathbb{M}: \exists \theta_m \in \mathcal{H}_m, s.t. f = f_{\theta_m} \}$ : $\mathcal{P}(\hat{m} = m_{*}) \rightarrow 1$ as $n \rightarrow \infty$
- parametric minimax risk over all candidate estimators $\hat{f}$ and true parameter $\theta_m$: $\mathcal{R}_n(m) = \inf_{\hat{f}} \sup_{\theta_m \in \mathcal{H}_m} \mathbb{E}_{\theta_m} [ \frac{1}{n} \sum\limits_{i=1}^n (f_{\theta_m}(x) - \hat{f}(x_i))^2 ]$
    - optimal for $C > 0, n \ge 1$: $\sup_{\theta_m \in \mathcal{H}_m} \mathbb{E}_{\theta_m} [ \frac{1}{n} \sum\limits_{i=1}^n (f_{\theta_m}(x) - \hat{f}(x_i))^2 ] \le C \cdot \mathcal{R}_n(m)$

- nonparametric minimax risk: $\mathcal{R}_n(\mathcal{F}) = \inf_{\hat{f}} \sup_{f \in \mathcal{F}} \mathbb{E}_{f} [ \frac{1}{n} \sum\limits_{i=1}^n (f(x) - \hat{f}(x_i))^2 ]$
    - optimal for $\tilde{C} > 0, n \ge 1$: $\sup_{f \in \mathcal{F}} \mathbb{E}_{f} [ \frac{1}{n} \sum\limits_{i=1}^n (f(x) - \hat{f}(x_i))^2 ] \le \tilde{C} \cdot \mathcal{R}_n(\mathcal{F})$

- Expected (over $\epsilon_n$) parametric prediction loss: $\mathbb{E}_{*} \lVert \bm{f}_n - \bm{f}_{\hat{\theta}_n} \rVert_2^2 = bias^2 + variance$
    - bias $\triangleq \lVert \bm{f}_n - F_n(m) \bm{f}_n \rVert_2$
    - variance $\triangleq \mathbb{E}_{*} (\epsilon_n^TF_n(m)\epsilon_n) = d_m \sigma^2$
- Residual Sum of Squares $RSS_m \triangleq \lVert \bm{y}_n - \bm{f}_{\hat{\theta}_m} \rVert_2^2 = \lVert \epsilon_n \rVert_2^2 + \lVert \bm{f}-n - \bm{f}_{\hat{\theta}_m} \rVert_2^2 - 2\epsilon_n^T F_n(m) \epsilon_n + 2 \epsilon_n^T (I - F_n(m))\bm{f}_n$
    - last term has zero mean, second-to-last doesnt so given $\epsilon_n \sim \mathcal{N}(0, \sigma^2 I)$ expectation is $2 Tr(F_n(m)) \sigma^2) = 2 d_m \sigma^2$
    - Under correct specification, second term vanishes.
    - Under correct specification, $\bm{f}_n$ is in column space of $X_m$, so the last term vanishes too.

### Intuition on Terms
- $F_n(m)$ being the "projection matrix of $y_n$ onto the column span of the predictors in model $\mathcal{M}_m$ means that $F_n(m) = X_m(X_m^TX_m)^{-1}X_m^T$ (least squares solution) 
    - eigenvalues of projection matrix are $1$ or $0$ and $rank(F_n(m))$ is dimension of column space of $X_m$
    - projection matrices map anything in the column space they project onto ($X_m$) to itself.

## Other Notes
