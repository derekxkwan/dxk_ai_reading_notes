---
title: "Predicting Music Hierarchies with a Graph-Based Neural Decoder"
date: 2026-02-02T13:45:57-08:00
authors: ["Francesco Foscarin", "Daniel Harasim", "Gerhard Widmer"]
year: 2023
tags: ["music theory", "dependency tree", "romantic period (music)", "graph", "baroque music", "classical period (music)", "graph neural network", "music", "jazz", "symbolic music", "hierarchical analysis", "harmonic analysis (music)", "harmony (music)", "gnn", "classical music"]
categories: ["supervised", "deep learning"]
paper_url: ""
doi: ""
paper_src: "Proceedings of the International Society for Music Information Retrieval Conference (ISMIR)"
bibkey: "foscarin_predicting_2023"
math: true
draft: false
---

## Summary
Predicts hierarchies of musical events (notes/chords) by calculating the most likely dependency tree. Consists of enriching a custom encoding scheme (pitches/chord quality/additions, duration, inverse metrical strength) with an encoder (map integers to continuous) and an arc predictor that predicts edges from head to dependent. Used on GTTM (generative theory of tonal music) databaseand JHT (jazz harmony treebank) datasets and optimized with BCE loss. Final tree calculated from MST.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

