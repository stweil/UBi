---
title: "RapidMiner Linked Open Data Extension: Integration of Web Knowledge into Data Mining"
source_url_de: N/A
source_url_en: https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/
category: Benutzung
tags: ['Linked Open Data', 'Data Mining', 'RapidMiner', 'Semantik', 'Feature Generation', 'SPARQL', 'Datenintegration']
language: en
---

# RapidMiner Linked Open Data Extension

The [RapidMiner](http://rapid-i.com/content/view/181/190/) [Linked Open Data](http://lod-cloud.net/) Extension is an extension for the open-source data mining software [RapidMiner](http://rapid-i.com/content/view/181/190/). It enables users to incorporate data from Linked Open Data sources both as primary input for data mining tasks and for enriching existing datasets with background knowledge.

This extension is based on the earlier [FeGeLOD framework](http://www.ke.tu-darmstadt.de/resources/fegelod) (which is now discontinued). The extension was the **Winner of the Semantic Web Challenge 2014**.

Unlike many related approaches, the extension can operate in a completely unsupervised manner, requiring minimal prior knowledge of the data source or technologies like RDF and SPARQL.

## Key Functionalities and Use Cases

The extension provides powerful capabilities for integrating external knowledge:

- **Data Importation**: Importing data from Linked Data sources (e.g., Eurostat) directly into RapidMiner for analysis using standard operators.
- **Background Knowledge Enrichment**: Adding contextual data to existing datasets. Examples include:
  - Adding population, GDP, and literacy data from Eurostat to country datasets.
  - Adding turnover and employee count data from DBpedia to company datasets.
- **Data Linkage and Discovery**:
  - Identifying potentially incorrect or missing links between datasets within Linked Open Data.
  - Analyzing relationships between datasets.
- **Advanced Applications**:
  - Predicting fuel consumption of cars.
  - Building hybrid recommender systems using Linked Open Data.
  - Generating features using Graph Kernels.

**Example Use Cases:**

- [Importing and analyzing data from Eurostat](https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-reading-and-analyzing-data-from-eurostat/)
- [Adding background data from Eurostat](https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-adding-background-data-from-eurostat/)
- [Adding background information from DBpedia](https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-adding-background-information-from-dbpedia-with-multiple-generators/)
- [Discovering wrong links between datasets](https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-discovering-wrong-links-between-datasets/)
- [Predicting car fuel consumption](https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-predicting-the-fuel-consumption-of-cars/)
- [Hybrid recommender system using Linked Open Data](https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-hybrid-recommender-system-using-linked-open-data/)
- [Using Graph Kernels for Feature Generation](https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-using-graph-kernels-for-feature-generation/)

## Technical Components (Operators)

The extension provides three main categories of operators that can be combined with built-in RapidMiner operators:

1. **Data Importers**: Load data from Linked Open Data into RapidMiner for subsequent processing.
1. **Linkers**: Create explicit links from a given dataset to a dataset within Linked Open Data (e.g., linking a CSV file to DBpedia).
1. **Generators**: Gather data from Linked Open Data and append it as new attributes to the current dataset.

Generators support various data additions, such as:

- Adding specific attributes (e.g., population).
- Adding categorical types (e.g., "G20 country").
- Adding aggregated relationships (e.g., number of companies in a city).

Furthermore, the extension allows for the addition of arbitrary data using customizable SPARQL statements.

## Installation and Documentation

**Download:**
The RapidMiner Linked Open Data Extension is available on the [RapidMiner marketplace](https://marketplace.rapid-i.com/UpdateServer/faces/product_details.xhtml?productId=rmx_lod).

**Installation Guide:**
To install the extension, navigate to the **“Help” $\\rightarrow$ “Updates and Extensions”** menu within RapidMiner and search for **“Linked Open Data”**.

**Documentation:**
All operators and example workflows are detailed in the [user manual (PDF, 995 kB)](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Projects/RapidMinerLODExtensionManual.pdf).

## Publications and Research

The underlying algorithms and the extension itself have been documented in several academic publications:

**Core Papers:**

- [Towards Linked Open Data enabled Data Mining: Strategies for Feature Generation, Propositionalization, Selection, and Consolidation (PDF)](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Petar_Ristoski_-_PhD_Symposium_ESWC_2015.pdf). In: Extended Semantic Web Conference, 2015.
- [Data Mining with Background Knowledge from the Web (PDF)](http://www.heikopaulheim.com/documents/rmworld_2014.pdf). In: RapidMiner World, 2014.
- [Exploiting Linked Open Data as Background Knowledge in Data Mining (PDF)](http://ceur-ws.org/Vol-1082/extendedAbstract.pdf). In: CEUR workshop proceedings DMoLD 2013.
- [Unsupervised Generation of Data Mining Features from Linked Open Data (PDF)](http://www.heikopaulheim.com/documents/wims2012.pdf). In: International Conference on Web Intelligence, Mining, and Semantics (WIMS), 2012.

**Application Examples:**

- **Identifying Wrong Links:** [Identifying Wrong Links between Datasets by Multi-dimensional Outlier Detection (PDF)](http://www.heikopaulheim.com/documents/wodoom_2014.pdf). In: WoDOOM 2014.
- **Statistical Analysis:**
  - [Generating Possible Interpretations for Statistics from Linked Open Data (PDF)](http://www.heikopaulheim.com/documents/eswc_2012.pdf). In: ESWC 2012.
  - [Analyzing Statistics with Background Knowledge from Linked Open Data (PDF)](http://www.heikopaulheim.com/documents/semstats_2013.pdf). In: SemStats 2013.
  - [Visual Analysis of Statistical Data on Maps using Linked Open Data (PDF, 896 kB)](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Web_Data_Mining/Ristoski_Paulheim_VisualAnalysisOfStatisticalDataOnMapsUsingLinkedOpenData.pdf). In: ESWC 2015.
- **Social Media & Event Classification:**
  - [I See a Car Crash: Real-time Detection of Small Scale Incidents in Microblogs (PDF)](http://www.heikopaulheim.com/documents/smile2013.pdf). In: SMILE 2013.
  - [A Multi-Indicator Approach for Geolocalization of Tweets (PDF)](http://www.heikopaulheim.com/documents/icwsm2013.pdf). In: ICWSM 2013.
  - [Automatic Classification and Relationship Extraction for Multi-Lingual and Multi-Granular Events from Wikipedia (PDF)](http://www.heikopaulheim.com/documents/derive2012.pdf). In: DeRiVE 2012.
- **Schema Matching:** [Towards Rule Learning Approaches to Instance-based Ontology Matching (PDF)](http://www.ke.tu-darmstadt.de/know-a-lod-2012/wp-content/uploads/2012/04/knowalod2012_submission_2.pdf). In: KnowALOD 2012.

## Support and Community

Users are encouraged to join the Google Group for support:
[https://groups.google.com/forum/#!forum/rmlod](https://groups.google.com/forum/#!forum/rmlod)

## Project Team

**Project Lead:**

- [Heiko Paulheim](https://www.uni-mannheim.de/dws/people/professors/prof-dr-heiko-paulheim/)

**Current Team Members:**

- [Christian Bizer](https://www.uni-mannheim.de/dws/people/professors/prof-dr-christian-bizer/)
- Evgeny Mitichkin
- Petar Ristoski

**Past Contributors:**

- Raad Bahmani
- [Johannes Fürnkranz](http://www.ke.tu-darmstadt.de/staff/juffi)
- Alexander Gabriel
- Simon Holthausen
