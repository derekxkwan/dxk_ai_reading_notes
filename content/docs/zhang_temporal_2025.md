---
title: "Temporal Adaptation of Pre-trained Foundation Models for Music Structure Analysis"
date: 2026-02-02T13:45:57-08:00
authors: ["Yixiao Zhang", "Haonan Chen", "Ju-Chiang Wang", "Jitong Chen"]
year: 2025
tags: ["convolutional", "music boundary", "music", "audio", "boundary detection (music)", "downsampling (audio)", "transformer", "fine-tuning", "non-bar/beat aligned similarity", "contrastive", "music theory", "popular music", "structure labeling (music)", "formal analysis (music)"]
categories: ["deep learning", "supervised"]
paper_url: "http://arxiv.org/abs/2507.13572"
doi: "10.48550/arXiv.2507.13572"
paper_src: "arXiv"
bibkey: "zhang_temporal_2025"
math: true
draft: false
---

## Summary
Explores fine-tuning a music foundation model MusicFM won\_foundation\_2024 based on the Conformer architecture using longer audio window inputs but downsampling using low-resolution adaptation (increasing hop size of mel-spectrogram input by multiplier $N$). Regularizes using contrastive learning where positive pairs are from the same section label. For label/structural function head, use weighted BCE loss. For boundary detection, use WBCE + smooth L-1 loss and focal loss.  Expr fine-tune on Harmonix, test on RWC-Pop (and vice versa) on cross-dataset, else results on separate datasets (just Harmonix). All-In-One model (other model from different paper) best on hit-rate boundary detection at 0.5 sec, else 150s ($N=3$) best on label acc, 100s $N=2$ best on HR3F. Cross-dataset, 180s ($N=2$) best on acc train on RWC-pop and 150s $N=3$ best on HR3F (MusicFM best on HR0.5F). 150s $N=3$ best on acc train on Harmonix, 100s $N=2$ best on HR3F, else no best given (underperforms on HR0.5F compared to all models). label acc improves with bigger window lengths (marginal over 50s) and $N \le 3$ but HR metrics decline for bigger window lengths (stable for any $N$).

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

