---
title: Datenanalyse von Linked Open Data (Eurostat) mit RapidMiner
source_url_de: https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-reading-and-analyzing-data-from-eurostat/
category: Benutzung
tags: ['RapidMiner', 'Eurostat', 'Linked Open Data', 'SPARQL', 'Datenimport', 'Korrelation', 'Datenanalyse']
language: en
---

# Reading and Analyzing Data from Eurostat Linked Open Data

This document provides an example of how to read and analyze data from the Linked Open Data source Eurostat using RapidMiner. The corresponding RapidMiner workflow can be downloaded from [myExperiment](http://www.myexperiment.org/workflows/3757.html).

The primary goal of this example is to read a list of countries, their GDP, and energy consumption from Eurostat and examine the correlation between GDP and energy consumption.

## Process Overview

The process involves several key steps within the RapidMiner environment:

1. **Defining the SPARQL Endpoint:** To access a Linked Open Data source like Eurostat, a SPARQL Endpoint must first be defined. This is done via the SPARQL Endpoint configuration dialog, accessible through the menu path: `Tools` $\\rightarrow$ `Manage SPARQL Connections`.
1. **Data Importation:** The `SPARQL Data Importer` operator is used to read the data. This operator requires two parameters:
   - The previously defined SPARQL endpoint.
   - A SPARQL query statement used to structure the resulting table.
1. **Data Structure:** Since the SPARQL statement contains three variables (country, GDP, and electricity), the resulting table is generated with three columns. RapidMiner automatically assigns data types: the country name is recognized as a text attribute, while GDP and electricity are correctly identified as numeric attributes (verifiable in the metadata view).
1. **Analysis:**
   - **Initial Assessment:** A scatter plot view in RapidMiner can be used to get a preliminary visual impression of the relationship between the variables.
   - **Formal Computation:** Wiring the output of the `SPARQL Data Importer` directly to the `Correlation Matrix` operator allows for a formal computation of the correlation coefficient.

## Results and Conclusion

The analysis reveals a strong correlation between the GDP and the energy consumption of European countries.

In summary, the RapidMiner Linked Open Data extension successfully enables users to read data from open data sources, such as Eurostat, and make this data accessible within RapidMiner for subsequent processing and analysis.
