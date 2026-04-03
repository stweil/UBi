---
title: Hybrid Recommender System using Linked Open Data and RapidMiner
source_url_de: None
source_url_en: https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-hybrid-recommender-system-using-linked-open-data/
category: Projekte
tags: ['Recommender', 'Linked Open Data', 'DBpedia', 'RapidMiner', 'Content-Based', 'Hybrid', 'SPARQL']
language: en
---

# Hybrid Recommender System Development with Linked Open Data

This document outlines the process of building a hybrid, Linked Open Data-enabled recommender system for books using RapidMiner. The system combines content-based recommendations derived from external knowledge graphs with collaborative filtering methods.

## 🛠️ Tools and Workflow Overview

The process utilizes the following key components:

- **Rapid Miner Linked Open Data extension:** For integrating external data sources.
- **Recommender extension:** For implementing recommendation algorithms.

The overall workflow can be visualized in the [RapidMiner workflow example](http://www.myexperiment.org/workflows/4285.html).

### Data Sources

The data used for this project was obtained from the [Linked Open Data-enabled Recommender Systems Challenge](https://link.springer.com/chapter/10.1007/978-3-319-12024-9_17).

- **Input Data:** The initial CSV file contains books already linked to [DBpedia](http://dbpedia.org/). Input data files can be downloaded [here](http://data.dws.informatik.uni-mannheim.de/rmlod/hybridrecommendersystem/input_data.zip).

## 📚 Feature Extraction from Linked Open Data (DBpedia)

The core of the content-based recommender relies on extracting rich features from [DBpedia](http://dbpedia.org/) using SPARQL queries.

### Feature Generation Process

1. **Initial Reading:** The process begins by reading the input CSV file, where books are linked to [DBpedia](http://dbpedia.org/).
1. **Generators Used:** Three generators are employed, all configured with the standard [DBpedia](http://dbpedia.org/) SPARQL endpoint:
   - Direct Types
   - Specific Relation
   - Custom SPARQL Generator
1. **Specific Relation:** This generator is used to extract the direct categories associated with each book in the dataset.
1. **Custom SPARQL Generator:** This advanced generator is used to retrieve complex relational data, such as:
   - Genres of the author.
   - Genres that influenced the author.
   - Genres of authors who influenced the current author, or authors influenced by the current author. (See [Figure 2](placeholder_for_figure_2) for an example query).

### Model Input Preparation

The outputs from all generators are joined into a single dataset. This dataset is then formatted for the item attribute-based k-NN operator of the Recommender extension.

- **Reference:** Detailed instructions on input formats and the Recommender extension can be found in the [extension manual (PDF)](http://zel.irb.hr/wiki/lib/exe/fetch.php?media=del:projects:elico:recsys_manual_v1.1.pdf).

## 🧠 Building the Recommender System

The system is built in two main stages: content-based modeling and collaborative modeling.

### 1. Content-Based Recommender

A content-based recommender is built using the **item attribute-based k-NN operator**. This model leverages *all* features generated from DBpedia.

### 2. Collaborative Recommenders

The training data, which contains user ratings for various books, is used to build two separate collaborative recommenders:

- User k-NN based recommender
- Item k-NN based recommender

### 3. Model Combination

Finally, the three components are integrated:

- The content-based recommender.
- The user k-NN recommender.
- The item k-NN recommender.

These three models are combined using the **Model Combiner operator** to produce a single, comprehensive model capable of predicting ratings for unseen books.
