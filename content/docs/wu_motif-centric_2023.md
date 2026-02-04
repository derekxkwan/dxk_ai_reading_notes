---
title: "Motif-Centric Representation Learning for Symbolic Music"
date: 2026-02-02T13:45:57-08:00
authors: ["Yuxuan Wu", "Roger B. Dannenberg", "Gus Xia"]
year: 2023
tags: ["motif (music)", "music theory", "midi", "popular music", "data augmentation", "contrastive learning", "music", "symbolic music", "contrastive", "vicreg", "neural network architecture development"]
categories: ["supervised"]
paper_url: "http://arxiv.org/abs/2309.10597"
doi: "10.48550/arXiv.2309.10597"
paper_src: "arXiv"
bibkey: "wu_motif-centric_2023"
math: true
draft: false
---

## Summary
Task is to learn embeddings suitable for embeddings (uses POP909 dataset, MIDI files)
Using VICReg-inspired pretraining  (trains on only positive pairs coming from data augmentation), learns initial embeddings based on invariance loss (positive pairs close), variance loss (induce variance within positive pairs), and covariance loss (ensure covariance of batched examples 0). Finetunes using contrastive learning.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

