---
title: "An Interactive Workflow for Generating Chord Labels for Homorhythmic Music in Symbolic Formats"
date: 2026-02-02T13:45:57-08:00
authors: ["Yaolong Ju", "Samuel Howes", "Cory McKay", "Nathaniel Condit-Schultz", "Jorge Calvo-Zaragoza", "Ichiro Fujinaga"]
year: 2019
tags: ["harmonic analysis (music)", "vocal instrumentation", "multi-task", "music", "chord labeling (music)", "human intervention", "svm", "ensemble methods", "mlp", "human-in-the-loop", "music theory"]
categories: ["classification", "unsupervised", "deep learning", "non-neural network"]
paper_url: "https://zenodo.org/records/3527950"
doi: "10.5281/zenodo.3527950"
paper_src: "International Society for Music Information Retrieval Conference (ISMIR 2019)
Pages: 862-869
Publication Title: Proceedings of the 20th International Society for Music Information Retrieval Conference
Publisher: ISMIR"
bibkey: "ju_interactive_2019"
math: true
draft: false
---

## Summary
Creates a workflow that uses a rule-based model that is used to (pre)-train an ensemble of three SVMs (or neural networks) to vote on chord labels (root + quality). When there is disagreement, a re-training step using "partial manual modification" is done for the ensemble and then the rule-based model is included in voting. First model indicates the presence of pitch classes, other two predict chord labels. Does better than all individiually, particularly after re-training. DNN without re-training does worse than rule-based alone, but better on re-training. Done on Bach chorales (modified by Craig Sapp)

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

