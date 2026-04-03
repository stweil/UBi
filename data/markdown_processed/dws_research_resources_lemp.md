---
title: LEMP Tool for Maximum Inner Product Search (MIPS)
source_url_de: https://www.uni-mannheim.de/dws/research/resources/lemp/
source_url_en: None
category: Services
tags: ['LEMP', 'Inner Product Search', 'Datensätze', 'Information Retrieval', 'SIGMOD', 'TODS', 'Matrix']
language: de
---

# LEMP: Exact and Approximate Maximum Inner Product Search

LEMP is a specialized tool designed for maximum inner product search (MIPS). This technique efficiently retrieves large entries within the product of two given large matrices. This problem is highly relevant in numerous data mining and information retrieval tasks.

For detailed technical descriptions and applications, please refer to the following publications:

- [SIGMOD 2015 paper](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/teflioudi15lemp.pdf)
- [TODS 2017 article](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/teflioudi16lemp-draft.pdf)

## Datasets

The project provides several pre-processed datasets for testing and research:

### IE-NMF Datasets

These datasets are based on Non-negative Matrix Factorization (NMF) and are available for ranks 10, 50, and 100:

- [IE-NMF-10](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/IE-nmf-10.tar.gz)
- [IE-NMF-50](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/IE-nmf-50.tar.gz)
- [IE-NMF-100](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/IE-nmf-100.tar.gz)

### IE-SVD Datasets

These datasets are based on Singular Value Decomposition (SVD) and are available for ranks 10, 50, and 100:

- [IE-SVD-10](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/IE-svd-10.tar.gz)
- [IE-SVD-50](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/IE-svd-50.tar.gz)
- [IE-SVD-100](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/IE-svd-100.tar.gz)

### Netflix Datasets

Datasets derived from the Netflix corpus, including versions with and without averaging:

- [Netflix-50](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/Netflix-50.tar.gz)
- [Netflix-noav-10](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/Netflix-noav-10.tar.gz)
- [Netflix-noav-50](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/Netflix-noav-50.tar.gz)
- [Netflix-noav-100](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/Netflix-noav-100.tar.gz)

### Glove Dataset

- [README](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/lemp-glove.tgz)

## Source Code

The source code for LEMP is available in two primary locations:

- **GitHub Repository:** The general source code is hosted on [LEMP GitHub repository](https://github.com/uma-pi1/LEMP).
- **Academic Versions:** Specific versions corresponding to the published papers are also available:
  - **SIGMOD Version:** [Download link](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/lemp-sources-sigmod.zip)
  - **TODS Version:** [Download link](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Software/LEMP/lemp-sources-tods.zip)
