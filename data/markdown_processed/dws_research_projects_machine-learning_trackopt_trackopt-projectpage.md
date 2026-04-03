---
title: "TrackOpt: Framework for Physically Constrained Point Tracking using Machine Learning"
source_url_de: https://www.uni-mannheim.de/dws/research/projects/machine-learning/trackopt/trackopt-projectpage/
category: Projekte
tags: ['Tracking', 'Machine Learning', 'Punktwolke', 'Optimierung', 'Deep Learning', 'Physik', 'Mikroskopie', 'Framework']
language: de
---

# TrackOpt: Learning to Optimize Physically Constrained Sparse-to-Dense Point Tracking

TrackOpt is a research project dedicated to developing an efficient and resilient framework for tracking individually occurring points or dense point clouds. This technology is highly relevant across various physical and biological domains, where tracking data often comes from limited, annotated datasets subject to measurement uncertainties.

The core objective is to create a flexible method framework that can reliably solve new tracking problems by integrating the strengths of two distinct approaches: **model-driven optimization** and **deep neural networks**.

## 🔬 Project Approach and Methodology

The framework is designed to be resilient and data-efficient by integrating domain knowledge directly into the learning process.

- **Hybrid Modeling:** Model-driven optimization problems are combined with deep neural networks. This integration allows the system to incorporate necessary physical or biological constraints for a valid solution, leading to high data efficiency.
- **Robustness:** The learned networks are specifically optimized to predict consistent solutions despite inherent measurement uncertainties and noise.
- **Application Scope:** The framework is built upon three primary fields of application:
  - Particle Physics
  - Microfluidics
  - Microscopy

## 🛠️ Software Toolbox

The project develops a reusable, transdisciplinary, and modular software toolbox. This tool is intended to be an open-source application, enabling external parties in diverse research and application areas to independently solve complex tracking problems, even with different boundary conditions.

## 🧑‍🔬 Research Team and Partners

The project involves collaboration across several leading German universities and research groups:

**University of Mannheim**

- Chair of Machine Learning: Prof. Margret Keuper, Dr. Steffen Jung

**Heinrich Heine University Düsseldorf**

- Chair of Machine Learning: Prof. Paul Swoboda, Malte Günnewig

**University of Siegen**

- Experimental Particle and Astroparticle Physics Group: Prof. Markus Cristinziani, Dr. Vadim Kostyukhin, Dr. Diptaparna Biswas
- Chair of Computational Sensorics: Prof. Ivo Ihrke, Jannis Maron

**Ilmenau University of Technology**

- Group of Engineering Thermodynamics: Prof. Christian Cierpka, Dr. Sebastian Sachs

## 💰 Funding

This project is funded by the BMBF (Grant ID: 01IS24074A-D) with the project carrier [DLR](https://www.softwaresysteme.dlr-pt.de/de/machine-learning-modelle.php) under the call “Flexible, resiliente und effiziente Machine-Learning-Modelle”.
