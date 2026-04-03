---
title: OLPBENCH – Open Link Prediction Benchmark
source_url_de: https://www.uni-mannheim.de/dws/research/resources/olpbench/
category: Services
tags: ['Open Link Prediction', 'Benchmark', 'Knowledge Graph', 'OPIEC', 'Daten', 'NLP']
language: en
---

# OLPBENCH: Open Link Prediction Benchmark

OLPBENCH is a large-scale benchmark designed for Open Link Prediction. It was derived from the state-of-the-art Open Information Extraction corpus (OPIEC) by Gashteovski et al. (2019).

The benchmark dataset is substantial, containing:

- 30 million open triples.
- 1 million distinct open relations.
- 2.5 million distinct mentions of approximately 800,000 entities.

## Understanding Open Link Prediction

Open Link Prediction is defined as the task of predicting missing entity mentions given an Open Knowledge Graph and a specific question structure.

**Process:**

1. The input consists of an Open Knowledge Graph and a question defined by an entity mention and an open relation (e.g., `(“NBC-TV”, “has office in”, ?)`)
1. The goal is to predict the missing entity mention (the answer).
1. A predicted mention is considered correct if it corresponds to the actual answer entity.

## Publication Details

The benchmark was introduced in the following publication:

- **Title:** Can We Predict New Facts with Open Knowledge Graph Embeddings? A Benchmark for Open Link Prediction
- **Authors:** Samuel Broscheit, Kiril Gashteovski, Yanjie Wang, Rainer Gemulla
- **Conference:** The 58th Annual Meeting of the Association for Computational Linguistics (ACL), 2020
- **Paper Link:** [ACL Anthology Link](https://www.aclweb.org/anthology/2020.acl-main.209.pdf)

## Data and Code Resources

Resources for utilizing the OLPBENCH corpus are available for download:

### 💾 Data Download

The OLPBENCH corpus includes all data used in the paper's experiments (training sets: THOROUGH, BASIC, SIMPLE; validation sets: ALL, MENTION, LINKED; and test sets).

- **Full Data:** [olpbench.tar.gz](http://data.dws.informatik.uni-mannheim.de/olpbench/olpbench.tar.gz)
  *(Note: Compressed size is ~2.4 GB; uncompressed size is ~7.9 GB)*

### 💻 Code Repository

The code required for creating OLPBENCH from OPIEC and for training the models discussed in the paper will be published on GitHub.

- **GitHub:** [https://github.com/samuelbroscheit](https://github.com/samuelbroscheit)
