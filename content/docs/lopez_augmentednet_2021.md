---
title: "AugmentedNet: A Roman Numeral Analysis Network with Synthetic Training Examples and Additional Tonal Tasks"
date: 2026-02-02T13:45:57-08:00
authors: ["Néstor Nápoles López", "Mark R. H. Gotham", "Ichiro Fujinaga"]
year: 2021
tags: ["convolutional", "multi-task", "data augmentation", "harmonic analysis (music)", "chroma", "cnn", "classical period (music)", "representation learning", "symbolic music", "representation leveraging", "roman numeral analysis", "rnn", "music", "neural network architecture development", "baroque music", "music theory", "instrumental orchestration", "roman numeral analysis (music)", "classical music"]
categories: ["classification", "deep learning", "supervised"]
paper_url: "https://doi.org/10.5281/zenodo.5624533"
doi: "10.5281/zenodo.5624533"
paper_src: "Proceedings of the 22nd International Society for Music Information Retrieval Conference"
bibkey: "lopez_augmentednet_2021"
math: true
draft: false
---

## Summary
Does automatic Roman Numeral Analysis  with classification subtasks (key, degree, quality, inversion, root) and alternative tasks (Common RN,harmonic rhythm,  bass, tonicization of key, and PC-set) using chroma through a CNN into two bidir GRUs. Classifies pitches by note name and pitch class to avoid ambiguity (C\# vs Db).  CNN (granularity of 32nd note) is designed with more filters and smaller window at beginning to focus on immediate time steps with less filters and bigger windows later on. Does augmentation through transposition and "texturization" from Roman numeral ground truth (realize not as block chords but splitting off bass, voicing high voice first, alberti bass, and mixing all of them randomly). Experiments on Annotated Beethoven Corpus, Beethoven Piano Sonatas, Haydn Sun Quartets, Theme and Variation Encodings with Roman Numerals, When-in-Roman, WTC. On main tasks, more augmentation = better (except for inversion) and for roman numeral prediction, alt tasks did better than main tasks. AugN state of the art compared to Micchi model and Chen and Su model.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

