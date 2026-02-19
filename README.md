# Comparative Analysis of Multiple Sequence Alignment Techniques

A comparative study of six Multiple Sequence Alignment (MSA) tools evaluated across standard bioinformatics benchmarks.

## Overview

This project benchmarks classical, graph-based, probabilistic, ensemble, and deep learning-based MSA methods to help researchers make informed tool selection decisions based on accuracy, computational efficiency, and biological relevance.

## Tools Evaluated

- **Clustal Omega** – Progressive alignment with guide tree
- **MUSCLE** – Iterative progressive alignment
- **MAGUS** – Graph clustering-based divide-and-conquer
- **MSA Probs** – Probabilistic pair-HMM approach
- **M-Coffee** – Consensus meta-aligner
- **MSA Transformer** – Deep learning with attention mechanisms

## Datasets

- BAliBASE (RV20, RV30, RV50)
- OXBench Master Set
- PREFAB 4.0

## Evaluation Metrics

- **SP Score** – Sum-of-Pairs (pairwise sensitivity)
- **TC Score** – Total Column accuracy
- **Q Score** – Overall alignment quality
- Runtime and memory usage
- Percent identity of conserved columns

## Key Findings

| Tool | Best At | Limitation |
|------|---------|------------|
| Clustal Omega | Closely related sequences | Poor on divergent data |
| MAGUS | Conserved datasets (SP: 100) | Low bio relevance on complex sets |
| M-Coffee | Balanced across datasets | High memory usage |
| MSA Probs | Perfect SP scores | Slow on complex inputs |
| MSA Transformer | Column accuracy, bio relevance | High compute cost |
| MUSCLE | — | Low accuracy, high resource use |
