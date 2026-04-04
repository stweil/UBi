---
title: "OPIEC: Open Information Extraction Corpus Details"
source_url_de: https://www.uni-mannheim.de/dws/research/resources/opiec/
source_url_en: https://www.uni-mannheim.de/dws/research/resources/opiec/
category: Medien
tags: ['Informationsextraktion', 'Korpus', 'Wikipedia', 'NLP', 'Daten', 'Triples', 'OIE']
language: en
---

# OPIEC: Open Information Extraction Corpus

OPIEC is an Open Information Extraction (OIE) corpus constructed from the entire English Wikipedia. It contains over 341 million triples. Each triple in the corpus is rich with metadata, including:

- NLP annotations (POS tag, NER tag, etc.) for every token in the subject, object, and relation.
- Provenance sentence details (including dependency parse and sentence order relative to the article).
- Original (golden) links contained within the Wikipedia articles, and space/time information.

For a detailed explanation of the metadata, please see the [OPIEC pipeline documentation](https://github.com/uma-pi1/OPIEC-pipeline#metadata).

## Datasets

The corpus is available in several versions, allowing users to select the appropriate level of data granularity:

### OPIEC Corpus Variants

| Corpus Version | Description | Full Data Download | Example File |
| :--- | :--- | :--- | :--- |
| **OPIEC-full** | The complete corpus. | [Full data](http://data.dws.informatik.uni-mannheim.de/opiec/OPIEC-full.zip) (~928.7 GB uncompressed) | [Example file](http://data.dws.informatik.uni-mannheim.de/opiec/OPIEC-Raw-example.avro) (~129 M) |
| **OPIEC-Clean** | Contains arguments considered "clean." | [Full data](http://data.dws.informatik.uni-mannheim.de/opiec/OPIEC-Clean.zip) (~292.4 GB uncompressed) | [Example file](http://data.dws.informatik.uni-mannheim.de/opiec/OPIEC-Clean-example.avro) (~40 MB) |
| **OPIEC-Linked** | Contains fully linked arguments. | [Full data](http://data.dws.informatik.uni-mannheim.de/opiec/OPIEC-Linked.zip) (~19.8 GB uncompressed) | [Example file](http://data.dws.informatik.uni-mannheim.de/opiec/OPIEC-Linked-example.avro) (~2.4 MB) |

### Bonus Corpus: WikipediaNLP

As an additional resource, we offer **WikipediaNLP**: the entire English Wikipedia enriched with NLP annotations (dependency parse, POS tags, NER tags, etc.).

- **Full data:** [Full data](http://data.dws.informatik.uni-mannheim.de/opiec/WikiNLP.zip) (~155 GB uncompressed)
- **Example file:** [Example file](http://data.dws.informatik.uni-mannheim.de/opiec/WikiNLP-example.avro) (~327 MB)

## Publications

- **OPIEC: An Open Information Extraction Corpus**
  Kiril Gashteovski, Sebastian Wanner, Sven Hertling, Samuel Broscheit, Rainer Gemulla.

  - [Conference Proceedings (AKBC, 2019)](https://openreview.net/pdf?id=HJxeGb5pTm)
  - [Author's Version (arXiv)](https://arxiv.org/abs/1904.12324)
  - [OpenReview Forum](https://openreview.net/forum?id=HJxeGb5pTm)

- **On Aligning OpenIE Extractions with Knowledge Bases: A Case Study**
  Kiril Gashteovski, Rainer Gemulla, Bhushan Kotnis, Sven Hertling, Christian Meilicke.

  - [ACL Proceedings (2020)](https://www.aclweb.org/anthology/2020.eval4nlp-1.14.pdf)
  - [Talk Slides (PDF)](https://www.uni-mannheim.de/media/Einrichtungen/dws/pi1/opiec/dsa-ota-talk-final.pdf)
  - [Resources](https://www.uni-mannheim.de/media/Einrichtungen/dws/pi1/opiec/opiec_dbpedia_study.zip)

## Code and Licensing

- **Code:**

  - Code for reading the data: [GitHub Repository](https://github.com/uma-pi1/OPIEC)
  - Code for the whole corpus construction: [GitHub Repository](https://github.com/uma-pi1/OPIEC-pipeline)

- **Licenses:**

  - All code is licensed under the [GPL-3.0 License](https://www.gnu.org/licenses/gpl-3.0.en.html).
  - All released data is licensed under the [Creative Commons Attribution Share-Alike license](https://en.wikipedia.org/wiki/Wikipedia:CCBYSA) (CC-BY-SA) and the [GNU Free Documentation License](https://en.wikipedia.org/wiki/Wikipedia:Text_of_the_GNU_Free_Documentation_License).
