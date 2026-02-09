---
title: "Modelling hierarchical key structure with pitch scapes"
date: 2026-02-02T13:45:57-08:00
authors: ["Robert Lieck", "Martin Rohrmeier"]
year: 2020
tags: ["harmonic analysis (music)", "hierarchical analysis", "pitch distribution", "music", "instrumental orchestration", "mixture models", "pitch (music)", "prototypes", "baroque music", "symbolic music", "mixture model", "music theory", "roman numeral analysis", "formal analysis (music)", "classical music"]
categories: ["non-neural network", "probabilistic", "supervised"]
paper_url: "https://doi.org/10.5281/zenodo.4245558"
doi: "10.5281/zenodo.4245558"
paper_src: "Proceedings of the 21st International Society for Music Information Retrieval Conference"
bibkey: "lieck_modelling_2020"
math: true
draft: false
---

## Summary
Learns pitch distributions (transposable per piece during training) per time bracket via mixture models (dirichlet pitch distributions). Starts by training one unified model for corpus (Baroque pieces) but then does binary splitting to initialize two prototypes (child clusters trained with weights of probability $p(d \_ c^{\prime})$ of piece $d$ falling into parent cluster $c^{\prime}$). Through this, they learn distributions of "prototypes" of pieces (key areas pieces visit). Big cluster has strong weights on circle of fifths. Child clusters cluster into minor/major then prototypes (i-III-i), then more fine prototypes (i-III-(VII)-v-III).

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

