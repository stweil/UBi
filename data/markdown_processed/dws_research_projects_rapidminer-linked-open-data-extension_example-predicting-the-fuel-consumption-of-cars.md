---
title: Vorhersage des Kraftstoffverbrauchs von Autos mittels Linked Open Data
source_url_de: https://www.uni-mannheim.de/dws/research/projects/rapidminer-linked-open-data-extension/example-predicting-the-fuel-consumption-of-cars/
category: Projekte
tags: ['Kraftstoffverbrauch', 'Auto', 'Vorhersage', 'Linked Open Data', 'DBpedia', 'RapidMiner', 'UCI', 'MPG']
language: en
---

# Predicting the Fuel Consumption of Cars using Linked Open Data

This example demonstrates how Linked Open Data can be utilized to improve the prediction of car fuel consumption.

**Resources:**

- **RapidMiner Workflow:** The corresponding RapidMiner workflow can be downloaded from [myExperiment](http://www.myexperiment.org/workflows/4284.html).
- **Dataset:** The data was obtained from the [UCI Auto MPG dataset](http://archive.ics.uci.edu/ml/datasets/Auto+MPG).
- **Input Data:** The input CSV file for the process can be downloaded [here](http://data.dws.informatik.uni-mannheim.de/rmlod/predictingfuelconsumption/auto-mpg.data).

The initial dataset contains car names and 8 other attributes, including the label attribute MPG (miles per gallon). This example proves that incorporating additional background knowledge from [DBpedia](http://dbpedia.org) for each car significantly improves the prediction accuracy.

## Methodology and Workflow

The overall workflow, depicted in Fig. 1, is divided into two sub-flows:

1. Predicting fuel consumption using only the initial dataset.
1. Predicting fuel consumption using additional knowledge extracted from DBpedia.

**Prediction Operator:**
For prediction, the [M5 Rules](http://weka.sourceforge.net/doc.dev/weka/classifiers/rules/M5Rules.html) operator, which is part of the [Weka extension](http://marketplace.rapid-i.com/UpdateServer/faces/product_details.xhtml?productId=rmx_weka), was used.

**Integrating External Knowledge (DBpedia):**
To link the car dataset to DBpedia, the **DBpedia Lookuplinker** was employed.

- **Query Class:** "Automobile" was used, utilizing the PrefixSearch API (as shown in Fig. 2).
- **Feature Generation:** The output of the linker was multiplied and passed to feature generators:
  - **Direct Typesgenerator:** Used for basic type extraction.
  - **Specific Relationgenerator:** Used to extract specific categories. In this generator, "http://purl.org/dc/terms/subject" was set as the desired relation (Fig. 3). Broader categories can be extracted by setting "http://www.w3.org/2004/02/skos/core#broader" for the hierarchy relation.

The outputs of both generators were joined into a single dataset. All attributes were then converted from nominal to numerical using the **Nominal to Numerical** step before performing 10-fold cross-validation on the M5 Rules.

## Results and Conclusion

The following table summarizes the performance metrics (Relative Error) for predicting fuel consumption using only the initial dataset versus the enhanced datasets. Linear Regression results are also reported.

**Key Findings:**

- The best prediction results are achieved when combining attributes derived from both direct types and categories.
- The new attributes provide insights not available from the original dataset alone. For instance:
  - UK cars were observed to have lower consumption compared to other regions (the original data only differentiated between America, Europe, and Asia).
  - Front-wheel-drive cars showed lower consumption than rear-wheel-drive ones (the corresponding category had a negative correlation with MPG at a level of 0.411), largely attributed to them being lighter.
  - A correlation between car design and consumption was noted (e.g., hatchbacks consuming less fuel than station wagons).
