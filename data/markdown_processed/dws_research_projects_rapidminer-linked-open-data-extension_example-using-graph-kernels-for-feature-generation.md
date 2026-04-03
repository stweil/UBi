---
title: Verwendung von Graph Kernels zur Feature-Generierung mit RDF-Daten
source_url_de: https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-using-graph-kernels-for-feature-generation/
category: Benutzung
tags: ['Graph-Kernel', 'RDF', 'RapidMiner', 'Feature-Generierung', 'DBpedia', 'Walk-Count', 'Weisfeiler-Lehman']
language: en
---

# Using Graph Kernels for Feature Generation with RDF Data

This document details an example demonstrating how to utilize graph kernels for feature generation, specifically using RDF data imported from DBpedia within the RapidMiner environment. The corresponding RapidMiner workflow can be downloaded from [myExperiment](http://www.myexperiment.org/workflows/4647.html).

## Understanding Graph Kernels for RDF Data

The RapidMiner LOD extension integrates two primary types of graph kernels designed for RDF data sourced from the [mustard library](https://github.com/Data2Semantics/mustard):

### 1. RDF Walk Count Kernel

This kernel calculates the count of distinct walks within subgraphs (up to a specified Graph Depth) surrounding the instance nodes. The maximum length of the walks considered is controlled by the **Walk Length** parameter.

- **Fast Approximation:** Provides a quick estimate of the total walks in the subgraph (using the *Full* setting).
- **Root:** Counts only walks that originate from the instance node (the root).
- **Tree:** Counts all walks within the subtree rooted at the instance node. This is computationally faster than the *Full* subgraph version because a tree structure lacks cycles.
- **Full:** Counts all walks in the entire subgraph. *(Note: This variant is typically very slow.)*

### 2. RDF WL Sub Tree Kernel

This kernel counts the different full subtrees within the subgraphs (up to a specified Graph Depth) using the Weisfeiler-Lehman (WL) algorithm. The maximum size of the subtrees is managed by the **Iterations** parameter.

- **Fast Approximation:** Provides a quick estimate of the total subtrees in the subgraph (using the *Full* setting).
- **Root:** Counts only subtrees starting from the instance node (the root). *(Note: This setting is included for completeness but may yield poor results.)*
- **Tree:** Counts all subtrees within the subtree rooted at the instance node. This is faster than the *Full* subgraph version because a tree structure lacks cycles.
- **Full:** Counts all subtrees in the entire subgraph.

## Implementation Workflow Example

In this specific example, the process utilizes the **Root RDF Walk Count Kernel** and the **Fast RDF WL Sub Tree Kernel**.

### Data Preparation

1. The process begins by reading a CSV file. This file contains a list of French regions, each labeled with an unemployment rate and including a DBpeida URI for that region.
1. The dataset can be obtained [here](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Web_Data_Mining/RapidMiner/completedataset.txt).

### Graph Import

1. The "Graph Importer" operator is used to import a sub-graph from DBpedia for the French regions.
1. **Configuration Details:**
   - The DBpedia endpoint is used.
   - The "DBpedia_URI" attribute is selected for extension.
   - The graph depth is set to 2.
   - The regular expression `"http://dbpedia.org/property.*"` is added to the "Properties to be avoid" parameter to exclude properties from the "dbprop" namespace.

### Kernel Application

1. The graph output from the "Graph Importer" operator is connected to the graph input port of the Kernel operators. This connection is also established for the ExampleSet.
1. Four specific graph kernel operators are configured and applied:
   - Root RDF Walk Count Kernel with a walk length of 2.
   - Root RDF Walk Count Kernel with a walk length of 3.
   - Fast RDF WL Sub Tree Kernel with a graph depth of 1 and 2 iterations.
   - Fast RDF WL Sub Tree Kernel with a graph depth of 2 and 2 iterations.

______________________________________________________________________

**References:**
[1] “A Fast and Simple Graph Kernel for RDF”, GKD de Vries and S de Rooij, DMoLD (2013).
[2] “A fast approximation of the Weisfeiler-Lehman graph kernel for RDF data”, GKD de Vries, Machine Learning and Knowledge Discovery in Databases, 606–621 (2013).
