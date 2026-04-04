---
title: "Supplementary Material: Theory and Algorithms for Rounding Rank"
source_url_de: https://www.uni-mannheim.de/dws/research/resources/rounding-rank/
category: Medien
tags: ['Rounding Rank', 'Matrixfaktorisierung', 'ICDM', 'Linearklassifikation', 'Dimensionsreduktion', 'Binärmatrizen', 'Algorithmen']
language: en
---

# Supplementary Material: Rounding Rank Theory and Algorithms

This page provides supplementary material for the paper, "What You Will Gain By Rounding: Theory and Algorithms for Rounding Rank," authored by Stefan Neumann, Rainer Gemulla, and Pauli Miettinen.

## Overview and Abstract

The paper addresses the challenge in factorizing binary matrices: choosing between computationally expensive combinatorial methods that preserve the discrete nature of the data, or efficient continuous methods that risk destroying this structure.

The core focus is on the concept of **rounding rank**. The authors investigate several key questions:

- Does rounding yield lower reconstruction errors?
- Is it straightforward to find a low-rank matrix that rounds to a given binary matrix?
- Does the choice of rounding threshold matter?
- Does restricting factorizations to non-negative values change the outcome?

The study demonstrates that rounding rank is related to linear classification, dimensionality reduction, and nested matrices. The paper also includes an extensive experimental study comparing various algorithms for finding optimal factorizations under the rounding rank model.

## Publications

**What You Will Gain By Rounding: Theory and Algorithms for Rounding Rank**

- **Authors:** S. Neumann, R. Gemulla, P. Miettinen
- **Publication Details:** To appear in ICDM, 2016
- **Links:**
  - [PDF Version](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/neumann16rr.pdf)
  - [Extended Version (arXiv)](https://arxiv.org/abs/1609.05034)

## Resources

For practical implementation and testing, the following resources are available:

- **Source Code and Synthetic Dataset Generators:** [tar.gz download](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/rounding_rank_code.tar.gz)
