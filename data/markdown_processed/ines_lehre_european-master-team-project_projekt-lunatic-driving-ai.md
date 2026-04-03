---
title: "Lunatic Driving AI: Benchmark Testing for Automated Test Case Generation"
source_url_de: None
source_url_en: https://www.uni-mannheim.de/en/ines/lehre/european-master-team-project/projekt-lunatic-driving-ai-1/
category: Projekte
tags: ['Software-Testing', 'KI', 'Automatisierung', 'Fahrsimulation', 'Testfallgenerierung', 'Machine Learning', 'Benchmark', 'ATCG']
language: en
---

# Lunatic Driving AI

This project centers on the field of automated test case generation (ATCG), a technique revolutionizing software testing by streamlining and optimizing the process. Traditionally, test case creation was manual and labor-intensive; ATCG has significantly increased speed, consistency, and overall testing effectiveness.

## Context: Automated Test Case Generation (ATCG)

The integration of AI and machine learning into ATCG is a major trend. Tools utilizing search-based software testing (SBST) allow testers to generate test cases that cover rare edge cases difficult to identify manually. Furthermore, AI introduces predictive analysis, enabling the prioritization of test scenarios based on bug probability.

**Challenge:** A major hurdle in this field is the effective evaluation and comparison of different testing approaches.

## Project Goal

The primary objective of this work is to create a comprehensive **benchmark testing environment** capable of evaluating machine-generated sets of test cases and assessing their coverage of the input space.

The core of the project will be a completely customizable driving AI.

### Required AI Capabilities

The driving AI must possess the following functionalities:

- **Safe Operation:** Ability to drive in a safe and controlled manner, adhering to speed limits, maintaining safe distances, and respecting traffic signals, other vehicles, and pedestrians.
- **Error Simulation:** Capability to execute subtle or drastic driving mistakes and safety violations across a broad variety of scenarios, based on predefined setups.
- **Malicious Behavior:** Ability to act as a complete "lunatic" and menace to society for rigorous testing purposes.

### Technical Specifications

**Programming Language:**

- The choice is up to the team.
- **Recommendation:** Python or C++ are recommended, given that CARLA (the simulation environment) is written in C++ and offers a versatile Python API.

**AI Model:**

- The approach is flexible.
- **Recommendation:** A rule-based approach is suggested, as integrating adjustable settings into a neural network or reinforcement learning-based AI can prove difficult.

**Frameworks:**

- Any framework, library, or open-source solution can be utilized, provided they possess reasonable licenses.
