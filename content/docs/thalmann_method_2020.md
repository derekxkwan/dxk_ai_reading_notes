---
title: "A method for analysis of shared structure in large music collections using techniques from genetic sequencing and graph theory"
date: 2026-02-02T13:45:57-08:00
authors: ["Florian Thalmann", "Kazuyoshi Yoshii", "Thomas Wilmering", "Wiggins Geraint", "Mark B. Sandler"]
year: 2020
tags: ["beat-aligned", "sequence alignment", "onset-aligned similarity", "hierarchical analysis", "pitch (music)", "hmm", "profile hmm", "beat-aligned similarity", "bioinformatics", "bar-aligned similarity", "musical form", "similarity graph", "chroma", "music theory", "formal analysis (music)", "msa", "bar-aligned", "music", "onset-aligned"]
categories: ["unsupervised", "non-neural network", "probabilistic"]
paper_url: "https://zenodo.org/records/4245440"
doi: "10.5281/zenodo.4245440"
paper_src: ""
bibkey: "thalmann_method_2020"
math: true
draft: false
---

## Summary
Performed over 15 Greatful Dead songs with multiple recordings from the Live Music Archive. Uses techniques inspired by bioinformatics and genetic sequencing. Creates an alignment graph (can be self-alignment) between two different (same) recordings of the same song by comparing beat/bar/onset aligned chroma or chord features using the Smith-Waterman algorithm (finds sections through similarity where here they limit to diagonals). Then creates a structure graph from alignments to find corresponding segments between different recordings in partitions using Profile HMMs (finds like sections called shared states, insert states are embellishments, delete states are things that can be omitted). Defines a structure graph that finds like partitions (verses, chorses, etc). Ground truths are lead sheets. Extracted chords (using madmom) okay but weakest, annotations second best, shared harmonic structure best (merges sequential partitions).

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

