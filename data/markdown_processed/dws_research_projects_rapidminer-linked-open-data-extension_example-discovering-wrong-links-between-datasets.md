---
title: Identifying Erroneous Links Between Datasets using Outlier Detection
source_url_de: None
source_url_en: https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-discovering-wrong-links-between-datasets/
category: Services
tags: ['Linked Open Data', 'Outlier Detection', 'Datenverknüpfung', 'Anomalieerkennung', 'SPARQL', 'DBpedia']
language: en
---

# Discovering Wrong Links Between Datasets using Outlier Detection

Links between datasets are crucial components of the [Linked Open Data cloud](http://lod-cloud.net/). Since manual link creation is not scalable, automatic tools like [Silk](https://wifo5-03.informatik.uni-mannheim.de/bizer/silk/) are often employed, though these tools may create links based on heuristics without guaranteeing 100% accuracy.

This example demonstrates how to use **outlier detection** to identify erroneous links between datasets. The process combines operators from the Linked Open Data extension with those from the [Anomaly Detection extension](http://madm.dfki.de/rapidminer/anomalydetection).

**Example Scope:**
The process reads and analyzes links between the [EventMedia dataset](https://eventmedia.eurecom.fr/) and [DBpedia](http://dbpedia.org/), aiming to identify errors within these connections. The full workflow is available from [myExperiment](http://www.myexperiment.org/workflows/4159.html).

## Methodology Overview

The overall process follows three distinct steps:

1. **Link Reading:** Reading the initial list of links between the two datasets.
1. **Feature Creation:** Generating descriptive features for the types of the linked resources from both sides.
1. **Outlier Identification:** Using outlier detection algorithms to pinpoint links whose type patterns deviate significantly from the established norm.

### Detailed Process Steps

**1. Reading Links (SPARQL Data Importer)**
The process begins by importing the list of links from the EventMedia dataset to DBpedia using the SPARQL data importer.

**2. Feature Generation**
Features are created for the direct types of both linked resources:

- **EventMedia Resources:** The Direct Types generator is used.
- **DBpedia Resources:** A custom SPARQL generator is employed to ensure that only types belonging to the DBpedia ontology are included.

**3. Outlier Detection (Local Outlier Factor)**
The **Local Outlier Factor (LOF)** operator from the Anomaly Detection extension is utilized. This operator identifies links whose pattern of resource types deviates significantly from the overall pattern observed in the dataset. The result is a list of links accompanied by a score, allowing users to sort and identify the most suspicious connections.

## Analysis of Results

Upon reviewing the results, the top 5 identified links contained several notable findings:

- **Incorrect Links:** Three of the top five links were confirmed to be factually wrong. Specifically, two links incorrectly associated rivers in DBpedia with music clubs of the same name in EventMedia.
- **True Outliers:** The remaining two elements in the top 5 were identified as outliers (a bridge and a library). While these locations are rare event venues, they were flagged as outliers by the algorithm despite being correct links.
