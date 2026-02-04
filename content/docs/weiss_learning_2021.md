---
title: "Learning Pitch-Class Representations from Score- Audio Pairs of Classical Music"
date: 2026-02-02T13:45:57-08:00
authors: ["Christof Weiss", "Johannes Zeitler", "Tim Zunner", "Florian Schuberth", "Meinard Müller"]
year: 2021
tags: ["harmonic cqt", "representation learning", "score-aligned (music)", "chord labeling (music)", "pitch (music)", "classical music", "cqt", "baroque music", "multi-pitch detection", "cnn", "chord recognition", "chroma", "classical period (music)", "neural network architecture development", "audio", "music theory", "romantic period (music)", "music", "multi-pitch recognition"]
categories: ["supervised", "deep learning"]
paper_url: "https://doi.org/10.5281/zenodo.5624549"
doi: "10.5281/zenodo.5624549"
paper_src: "Proceedings of the 22nd International Society for Music Information Retrieval Conference"
bibkey: "weiss_learning_2021"
math: true
draft: false
---

## Summary
learns a score/audio aligned representation for pitch classes for the downstream task of multi-pitch detection (but tested on chord recognition as well). Uses annotated scores (sometimes MIDI files) as ground truth pitch classes aligned with audio performances of music (MusicNet, Schubert Winterreise, Beethoven Sonatas Dataset, Der Ring des Nibelungen/Die Walkure). Input is the audio in form of HCQT (harmonic CQT with harmonic ratios above normal CQT bins on channel axis) with 3 bins per semitone for 72 semitones (6 octaves). has a prefiltering layer for vibrato, binning to MIDI pitch (3 x3, one for each semitone), time reduction (reduce down to 10 feature maps), Chroma reduction (merge channels using 1x1 conv) and then bin reduction (72 - 11 = 61) all with leaky ReLU. Ablations with more channels (5x each conv layer, Wide) and with inception layers (diff kernel sizes in one layer). Evaluation is done for multi-pitch on same and cross-dataset testing. Good results with Basic (F=0.832, Cosine Sim = 0.836 on SWD), best cross reults testing on a mix of subsets from all datasets testing on SWD. Almost matching chroma rep (Pscore) on chord rec but does not beat training on chord annotations themselves (extra step of functional analysis).

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

