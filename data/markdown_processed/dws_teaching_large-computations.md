---
title: Rechenressourcen für Studierende der Universität Mannheim
source_url_de: https://www.uni-mannheim.de/dws/teaching/large-computations/
category: Services
tags: ['Rechenleistung', 'Student', 'bwHPC', 'GPU', 'bwCloud', 'Datenverarbeitung', 'Cluster', 'Forschung']
language: de
---

# Compute Resources for Students at the University of Mannheim

This guide provides an overview of the computational resources available to students at the University of Mannheim for performing large-scale computations, such as those required for team projects or master theses.

**Important Note:** Please attempt to run your computations on your private machine first. Only utilize the external resources listed below if this proves unfeasible.

## 💻 Large-Scale Data Processing (HPC)

For processing large amounts of data or executing time-consuming computations, the **bwHPC** infrastructure is available.

- **bwUniCluster:** Students can utilize the [bwUniCluster](https://wiki.bwhpc.de/e/BwUniCluster2.0/Hardware_and_Architecture) for free. A brief project description is required for access.
- The available nodes and their hardware configurations are detailed on the [bwHPC Wiki](https://wiki.bwhpc.de/e/BwUniCluster2.0/Hardware_and_Architecture).

## 🚀 GPU Computations

The bwUniCluster also provides access to machines equipped with NVIDIA GPUs, enabling computations using CUDA.

- **GPU Usage Information:** Detailed instructions for using the GPUs can be found at the [bwUniCluster-Wiki](https://wiki.bwhpc.de/e/BwUniCluster2.0/Slurm#GPU_jobs).
- **JupyterLab Integration:** There is also an option to use the GPUs within a JupyterLab environment via the [bwUniCluster-JupyterLab](https://wiki.bwhpc.de/e/BwUniCluster2.0/Jupyter).

## 🖥️ Dedicated Linux Machine (Application Development)

If your goal is to develop an application that needs to be put online, or if you require a dedicated Linux environment for specific tasks, you can use [bwCloud](https://www.bw-cloud.org/en/first_steps).

- **Limitation:** Please note that GPUs cannot currently be used within the [bwCloud](https://www.bw-cloud.org/en/first_steps) environment.

## ⚠️ Fallback Option: Local Hardware

If neither bwHPC nor bwCloud meets your computational needs, you may consider using local hardware. This should be treated as the last resort, as these resources are quite limited. For guidance on this option, please consult your supervisor or professor.
