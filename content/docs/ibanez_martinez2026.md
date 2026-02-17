---
title: "Evaluating Disentangled Representations for Controllable Music Generation"
date: 2026-02-16T16:37:52-08:00
authors: ["Laura Ibáñez-Martı́nez", "Chukwuemeka Nkama", "Andrea Poltronieri", "Xavier Serra", "Martı́n Rocamora"]
year: 2026
tags: ["music", "music theory", "evaluation", "distentangled representations", "autoencoder", "variational autoencoder", "diffusion", "equivariance", "invariance", "probing", "generative"]
categories: ["evaluation", "supervised"]
paper_url: ""
doi: ""
paper_src: "ICASSP"
bibkey: "ibanez_martinez2026"
math: true
draft: false
---

## Summary
Evaluates the distentaglement of timbre (global) and structure (local) studying three generative models that encoder global and local features separately: SS-VQ-VAE (content/style), TS-DSAE (local/global), and AFTER(structure/timbre). Studies P-equivariance (equivariance in terms of predicted transformation parameters) and R-equivariance (equivariance of predicted transformed embedding) as well as invariance. 

Trained on Slakh2100 music separation dataset and probed using SynTheory. Multi-pitch estimation task trained using MAESTRO dataset.

Embedding size predictive of informativeness. Negative corr. between informativeness and embedding size. Strong entanglement with timbre and tempo. (Adversarial) loss functions and data augmentation helpful.

## Key Contributions
Study of entanglement through studying two-embedding models. 

## Limitations and Future Work
Disentanglement also depends on "decoding strategies" (needs "controlled generation experiments", "perceptual listening-based assessments").

## Key Equations

Equivariance: $ z(t(x)) \approx \rho_t(z(x))$

($ z = f(x)$ embedding, $\rho_t$ transformation in embedding space, transformation $t(x)$)

Entanglement measure: $ \Delta = | Acc(g^{\prime}(z_t \oplus z_s)) - Acc(g(z_t))| $

($z_t$ timbre embedding, $z_s$ structure embedding)


## Other Notes
