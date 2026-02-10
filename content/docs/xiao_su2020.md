---
title: "Detection of Local Boundaries of Music Scores with BLSTM by using Algorithmically Generated Labeled Training Data of GTTM Rules"
date: 2026-02-10T00:01:07-08:00
authors: ["You-Cheng Xiao", "Alvin Wen-Yu Su"]
year: 2020
tags: ["gttm", "generative", "music theory", "music", "symbolic music", "lstm", "bilstm", "rnn", "music analysis", "monophonic"]
categories: ["deep learning", "supervised"]
paper_url: "http://www.studiomusicatreviso.it/icnmc/library/Paper_77_2020.pdf"
doi: ""
paper_src: "Proceedings of the 7th International Conference on New Music Concepts"
bibkey: "xiao_su2020"
math: true
draft: false
---

## Summary
Trains a BiLSTM on data generated with music21 to test for GTTM's Grouping Preference Rules GPR 2a, 2b, 3a (register change), 3b (dynamic change), 3c (articulation change), 3d (note length) called LMS. Notes are randomized. Compared with ATTA (automatic time span tree analyzer), mostly performs better. Weaknesses on performance on GTTM dataset include lack of articulations/expressive markings that GTTM dataset has (trills). ATTA cannot handle slurs and has a weaker performance on GPR2a. 



## Key Contributions
BiLSTM trained to detect GPR 2a, 2b, 3a, 3b, 3c, 3d.

## Limitations and Future Work


## Key Equations


## Other Notes
