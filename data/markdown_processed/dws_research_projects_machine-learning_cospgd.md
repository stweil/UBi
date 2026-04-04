---
title: "CosPGD: Efficient White-Box Adversarial Attack for Pixel-wise Prediction Tasks"
source_url_de: https://www.uni-mannheim.de/dws/research/projects/machine-learning/cospgd/
source_url_en: https://www.uni-mannheim.de/dws/research/projects/machine-learning/cospgd/
category: Projekte
tags: ['Adversarial Attack', 'Segmentierung', 'Pixel-weise', 'Robustheit', 'Machine Learning', 'PGD', 'CosPGD']
language: en
---

# CosPGD: An Efficient White-Box Adversarial Attack for Pixel-wise Prediction Tasks

This work introduces **CosPGD**, an efficient adversarial attack designed for pixel-wise prediction tasks, aiming to improve model robustness evaluation beyond traditional point-wise attacks.

## 💡 Overview and Contribution

While neural networks achieve high accuracy, their lack of robustness to minor input perturbations is a major deployment hurdle. Existing attacks, like Projected Gradient Descent (PGD), are effective but often focus on isolated point-wise predictions. This can lead to optimization instability when trying to balance the attack across the entire image domain.

**CosPGD** addresses this by encouraging more balanced errors across the entire image domain while significantly increasing the attack's overall efficiency. It achieves this by leveraging a simple, fully differentiable alignment score computed between any pixel-wise prediction and its target.

CosPGD provides efficient evaluations for:

- Semantic Segmentation
- Regression models (e.g., Optical Flow, Disparity Estimation, Image Restoration)

The method has been shown to outperform previous State-of-the-Art (SotA) attacks on semantic segmentation.

## 🔬 Methodology: Prediction Alignment Scaling

The core innovation lies in the **Prediction Alignment Scaling** mechanism.

When testing on semantic segmentation using DeepLabV3 on the PASCAL VOC 2012 validation set, the stability of the attack was analyzed:

- **PGD** and **Seg[PGD]** showed large and increasing absolute differences in gradient values over attack iterations.
- **CosPGD** maintained stable gradient values and exhibited fewer changes in gradient direction compared to PGD and Seg[PGD], demonstrating superior optimization stability.

## 🧪 Applications and Demonstrations

CosPGD was validated across multiple challenging tasks:

### Semantic Segmentation

CosPGD was tested against models like [SegFormer](https://github.com/NVlabs/SegFormer) using the [ADE20K](https://groups.csail.mit.edu/vision/datasets/ADE20K/) dataset. When compared to [Seg[PGD]](https://openreview.net/pdf?id=BJm4T4Kgx), [PGD], and CosPGD as untargeted attacks, **CosPGD outperformed all other attacks** across various $\\ell\_\\infty$ bounded $\\epsilon$ values and attack iterations.

### Optical Flow Estimation

The attack was compared against PGD using the [Sintel (clean) validation dataset](http://sintel.is.tue.mpg.de/) for targeted $\\ell\_\\infty$-norm constrained 40-iteration attacks on [RAFT](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123470392.pdf).

## 🔗 Resources and Links

- **Paper:** [arXiv:2302.02213](https://arxiv.org/abs/2302.02213)
- **Code Repository:** [CosPGD Code and Sample Implementation](https://github.com/shashankskagnihotri/cospgd)
- **Segmentation Integration:** [CosPGD integrated with mmsegmentation](https://github.com/shashankskagnihotri/adv_mmsegmentation)
- **Presentation Slides:** [ICML 2024 Slides (PDF)](https://www.uni-mannheim.de/media/Einrichtungen/dws/Files_Research/Machine_Learning/Projects/cospgd_presentation_ICML2024_slides_upload.pdf)

## 🧑‍🏫 Authors and Acknowledgements

**Authors:**

- [Shashank Agnihotri](https://www.uni-mannheim.de/dws/people/researchers/phd-students/shashank/)
- [Steffen Jung](https://jung.vision/)
- [Prof. Dr.-Ing. Margret Keuper](https://www.uni-mannheim.de/dws/people/professors/prof-dr-ing-margret-keuper/)

**Funding:**
Steffen Jung and Margret Keuper acknowledge funding by the [DFG Research Unit 5336 – Learning to Sense](https://www.learning2sense.de/).
Initial computations utilized the [OMNI cluster of University of Siegen](https://cluster.uni-siegen.de/?lang=en).

______________________________________________________________________

*Note: This work was accepted at ICML 2024.*
