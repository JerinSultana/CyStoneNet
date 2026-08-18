# CyStoneNet: Pseudo-Color Enhanced SE-Attention MobileNetV2 for Kidney Stone and Cyst Detection

[![IEEE Xplore](https://img.shields.io/badge/IEEE-Xplore-blue?style=flat-square)](https://ieeexplore.ieee.org/document/11491240)
[![Python](https://img.shields.io/badge/Python-3.10%2B-green?style=flat-square)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-red?style=flat-square)](https://pytorch.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

Official PyTorch implementation of our research paper published in **IEEE Xplore**.

**Author:** Jerin Sultana,Joyita Sen,Nowshin Tasnim,Mohammed Mahmudur Rahman  
**Institution:** University of Science and Technology Chittagong (USTC)

---

## 📌 Abstract
Early and precise identification of renal abnormalities is crucial for effective clinical decision-making. **CyStoneNet** introduces a lightweight, robust deep learning framework specifically designed for automated renal disease classification using CT and Ultrasound images. By integrating a **Pseudo-Color Enhancement** preprocessing technique to boost low-contrast feature visibility alongside a **Squeeze-and-Excitation (SE) Attention-embedded MobileNetV2** backbone, our model accurately classifies medical images into three distinct diagnostic categories: **Normal**, **Cyst**, and **Stone**.

---

## 🏗️ Proposed Architecture
*(এখানে আপনার মডেলের পাইপলাইন বা ফ্লোচার্ট ইমেজ যুক্ত করতে পারেন, যেখানে Normal, Cyst এবং Stone—এই তিনটি ক্লাসের ক্লাসিফিকেশন প্রসেস দেখানো থাকবে)*
<p align="center">
  <img src="architecture_flowchart.png" width="850" alt="CyStoneNet Architecture">
</p>

---

## 🗂️ Repository Structure
```text
CyStoneNet/
│
├── dataset/                  # Dataset description and sample links
├── preprocess/               # Pseudo-color enhancement scripts
├── models/                   # MobileNetV2 + SE-Attention network architecture
├── weights/                  # Pre-trained model weights (.pth)
├── architecture_flowchart.png# Workflow/Architecture diagram
├── train.py                  # Training script
├── evaluate.py               # Evaluation and performance metrics script
├── requirements.txt          # Required Python packages
└── README.md                 # Project documentation
