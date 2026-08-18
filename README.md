# CyStoneNet: Pseudo-Color Enhanced SE-Attention MobileNetV2 for Kidney Stone and Cyst Detection

[![IEEE Xplore](https://img.shields.io/badge/IEEE-Xplore-blue?style=flat-square)](https://ieeexplore.ieee.org/document/11491240)
[![Python](https://img.shields.io/badge/Python-3.10%2B-green?style=flat-square)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?style=flat-square)](https://www.tensorflow.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

Official implementation of our research paper published in **IEEE Xplore (ICCIT 2025)**.

**Authors:** Jerin Sultana, Joyita Sen, Nowshin Tasnim, and Mohammed Mahmudur Rahman  
**Institution:** University of Science and Technology Chittagong (USTC)

---

## Abstract
Early and precise identification of renal abnormalities is crucial for effective clinical decision-making. This article proposed a lightweight framework for the detection of kidney disease from computed tomography scans. By applying pseudo-color modification to grayscale CT scans, the technique improves textural and spatial information that is sometimes missed in the conventional grayscale format. Moreover, the MobileNetV2 architecture is incorporated with a squeeze-and-excitation (SE) attention mechanism to adaptively highlight the most discriminative channel-wise features, accurately classifying medical images into three distinct diagnostic categories: **Normal**, **Cyst**, and **Stone**.

---

## Proposed Architecture
<p align="center">
  <img src="architecture_flowchart.png" width="850" alt="CyStoneNet Architecture">
</p>

---

## Preprocessing & Data Augmentation

### 1. Pseudo-Color Enhancement
To improve the textural and spatial information of the medical scans, grayscale CT scans are transformed into enhanced pseudo-color representations using OpenCV's JET colormap across three categories (**Cyst**, **Stone**, and **Normal**):

<p align="center">
  <img src="preprocessing_samples.png" width="950" alt="Preprocessing Samples - Original vs Pseudo Color">
</p>

### 2. Data Augmentation
To improve the generalization capability of the model and prevent overfitting, data augmentation techniques (such as rotation and spatial transformations) were applied to the pseudo-color enhanced images:

<p align="center">
  <img src="data_augmentation.png" width="950" alt="Data Augmentation Samples">
</p>

---

## Repository Structure
```text
CyStoneNet/
│
├── architecture_flowchart.png             # Workflow/Architecture diagram
├── preprocessing_samples.png              # Original vs Pseudo-color visualization
├── data_augmentation.png                  # Data augmentation samples
├── mobilenet_with_pseudocolor_enhancement.py # Complete implementation script
└── README.md                              # Project documentation

@inproceedings{sultana2025cystonenet,
  title={CyStoneNet: Pseudo-Color Enhanced SE-Attention MobileNetV2 for Kidney Stone and Cyst Detection},
  author={Sultana, Jerin and Sen, Joyita and Tasnim, Nowshin and Rahman, Mohammed Mahmudur},
  booktitle={2025 28th International Conference on Computer and Information Technology (ICCIT)},
  pages={4723--4728},
  year={2025},
  organization={IEEE}
}
