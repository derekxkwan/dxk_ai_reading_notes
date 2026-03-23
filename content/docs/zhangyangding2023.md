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


## Key Contributions


## Limitations and Future Work


## Key Equations
- consistency for $m_{*} = \arg \min_{m \in \mathbb{M}_w} d_m$ where $\mathbb{M}_w \triangleq \{ m \in \mathbb{M}: \exists \theta_m \in \mathcal{H}_m, s.t. f = f_{\theta_m} \}$ : $\mathcal{P}(\hat{m} = m_{*}) \rightarrow 1$ as $n \rightarrow \infty$
- parametric minimax risk over all candidate estimators $\hat{f}$ and true parameter $\theta_m$: $\mathcal{R}_n(m) = \inf_{\hat{f}} \sup_{\theta_m \in \mathcal{H}_m} \mathbb{E}_{\theta_m} [ \frac{1}{n} \sum\limits_{i=1}^n (f_{\theta_m}(x) - \hat{f}(x_i))^2 ]$
    - optimal for $C > 0, n \ge 1$: $\sup_{\theta_m \in \mathcal{H}_m} \mathbb{E}_{\theta_m} [ \frac{1}{n} \sum\limits_{i=1}^n (f_{\theta_m}(x) - \hat{f}(x_i))^2 ] \le C \cdot \mathcal{R}_n(m)$

- nonparametric minimax risk: $\mathcal{R}_n(\mathcal{F}) = \inf_{\hat{f}} \sup_{f \in \mathcal{F}} \mathbb{E}_{f} [ \frac{1}{n} \sum\limits_{i=1}^n (f(x) - \hat{f}(x_i))^2 ]$
    - optimal for $\tilde{C} > 0, n \ge 1$: $\sup_{f \in \mathcal{F}} \mathbb{E}_{f} [ \frac{1}{n} \sum\limits_{i=1}^n (f(x) - \hat{f}(x_i))^2 ] \le \tilde{C} \cdot \mathcal{R}_n(\mathcal{F})$
 
## Other Notes
