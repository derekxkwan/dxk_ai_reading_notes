---
title: "Audio synthesizer inversion in symmetric parameter spaces with approximately equivariant flow matching"
date: 2026-02-02T13:45:57-08:00
authors: ["Ben Hayes", "Charalampos Saitis", "György Fazekas"]
year: 2025
tags: ["flow matching", "normalizing flows", "synth parameters", "diffusion", "inversion", "audio", "synthesizer", "group theory", "mel spectrogram", "neural network architecture development", "transformer", "weight tying"]
categories: ["diffusion", "deep learning", "supervised"]
paper_url: ""
paper_type: ""
doi: "10.5281/zenodo.17706418"
paper_src: "Proceedings of the 26th International Society for Music Information Retrieval Conference"
bibkey: "hayes2025"
math: true
draft: false
---

## Summary
Using group theory assumptions, considers the transformations that map within parameters that map to the same sound as an orbit. Uses that to derive a conditional probability and inform an isotropic gaussian noising (whose pushforward preserves equivariant). Parameterizes normalizing flow model with a proposed Param2Tok transformer model that utilizes weight tying. Trained with L1 loss on a assignment track from tokens. Performs better that baseline audio spectrogam and  VAE baselines.
## Key Contributions
Param2Tok conditional normalizing flow model and that encodes equivariances of parameter ambiguity (different ordering of parameters yielding same output sound).

## Limitations and Future Work
Lack of theoretical study (there is plenty though) and lack of generalizing to different synthesizers.

## Key Equations

## Other Notes
