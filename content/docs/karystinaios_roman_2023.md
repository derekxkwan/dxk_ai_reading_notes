---
title: "Roman Numeral Analysis with Graph Neural Networks: Onset-Wise Predictions from Note-Wise Features"
date: 2026-02-02T13:45:57-08:00
authors: ["Emmanouil Karystinaios", "Gerhard Widmer"]
year: 2023
tags: ["music theory", "graphsage", "instrumental orchestration", "multi-task", "baroque music", "classical period (music)", "graph neural network", "roman numeral analysis", "music", "symbolic music", "roman numeral analysis (music)", "representation leveraging", "harmonic analysis (music)", "neural network architecture development", "gnn", "classical music"]
categories: ["supervised", "classification", "deep learning"]
paper_url: ""
doi: ""
paper_src: "Proceedings of the International Society for Music Information Retrieval Conference (ISMIR)"
bibkey: "karystinaios_roman_2023"
math: true
draft: false
---

## Summary
with heterogenous edges (same onset, note sounding during sustain, next sequential, next after rest) and adding a contraction layer that pools all notes with same onsets. From that, they get a sequence which is projected using an MLP and then fed into GRU for predictions on tassks (MLP). New predictions come from feeding trained logits on all tasks concatenated into BiLSTM and then feeding into separate MLPs. Trained on Annotated Beethoven Corpus, annotated Beethoven Piano Sonatas, Hadyn String Quartets, TAVERN, When-in-Rome, WTC. For BPS, test on first movements or full (7 beethoven piano sonatas). On partial BPSAugmented Net does best on all subtacks besides Inversion (current with post proc for new predictions) (80s-70s). Roman Numeral (particularly on onset), current with post proc best. On Full BPS, AugNet best on Key and Qual, current + post better on other subtasks (degree, inversion, root), again, best on all Roman Numeral tasks (50s). Better performance when trained on additional subtasks from Napoles Lopez PhD.

## Key Contributions

## Limitations and Future Work

## Key Equations

## Other Notes

