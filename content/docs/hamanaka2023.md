---
title: "deepGTTM-IV: Deep Learning Based Time-span Tree Analyzer of GTTM"
date: 2026-02-13T11:33:13-08:00
authors: ["Masatoshi Hamanaka", "Keiji Hirata","Satoshi Tojo"]
year: 2023
tags: ["gttm", "music analysis", "hierarchical music analysis", "music segmentation", "symbolic music", "transformer", "music", "music theory", "monophonic", "music formal analysis"]
categories: ["deep learning", "supervised"]
paper_url: "https://gttm.jp/hamanaka/wp-content/uploads/2024/06/cmmr2023_4e-1-DeepGTMIV.pdf"
doi: ""
paper_src: "Proceedings of CMMR2023, the 16th International Symposium on Computer Music Multidisciplinary Research"
bibkey: "hamanaka2023"
math: true
draft: false
---

## Summary
Uses a transformer model to learn a time-span (binary) tree representation (establishes a hierarchy of notes) as formulated in GTTM. Transformer model learns a single-note reduction method that is fed back into the transformer until one note is left. Note salience is determined by the duration of the branch. If errors are found, initial duration is multiplied by a multiple of 2 and the process is restarted. Tree is represented in a matrix format with first row being pitch class with duration (subdivision multiplied by 4 rounded to nearest integer in terms of tuples). Second row is parent branch by note number (notes in distinct lower branches may share same parent). Third row is priority (smaller = higher, unique). Reduced notes are blanked out in first row. Accuracy is 0.99over 849 stepwise reductions. 

## Key Contributions
Transformer model to recursively remove notes to predict a time-span tree.

## Limitations and Future Work
(not stated) Process is recursive, would be nice to not have to keep feeding step-wise reductions back into transformer.

## Key Equations


## Other Notes
