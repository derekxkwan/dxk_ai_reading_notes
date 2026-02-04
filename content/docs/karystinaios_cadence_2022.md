---
title: "Cadence Detection in Symbolic Classical Music using Graph Neural Networks."
date: 2026-02-02T13:45:57-08:00
authors: ["Emmanouil Karystinaios", "Gerhard Widmer"]
year: 2022
tags: ["handcrafted features", "music theory", "graphsage", "instrumental orchestration", "cadence detection (music)", "smote", "baroque music", "classical period (music)", "graph neural network", "music", "symbolic music", "harmonic analysis (music)", "data augmentation", "neural network architecture development", "oversampling (audio)", "gnn", "classical music"]
categories: ["deep learning"]
paper_url: "https://doi.org/10.5281/zenodo.7316814"
doi: "10.5281/zenodo.7316814"
paper_src: "Proceedings of the 23rd International Society for Music Information Retrieval Conference"
bibkey: "karystinaios_cadence_2022"
math: true
draft: false
---

## Summary
) binary classification (yes/no cadence) via aggregation (?). Experiments include pretraining on more data (str qtr when testing on bach and other way around). Usu competitive but Bigo better at F1 and Precision on Bach for PAC (pretrained best with recall), non pre-trained best on rIAC on Bach (pretrained best on recall), Bigo best F1/Prec/Recall for PAC on Haydn, Pretrained best on F1/Prec on HC (Bigo best on recall). So generally Bigo best on PAC, SMOTE otherwise (and pretrained generally better than non-pretrained except for rIAC on Bach). HC still hard (around .4 accuracy for pretrained). Depth of GNN increasing number of hops in graph to consider and hops=2 the best (vanishing gradient problem in GNNs)

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

