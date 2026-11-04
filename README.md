# SDU Deep Learning (DM873 / DS809) — Project 1
## Cat & Dog Classification with Convolutional Neural Networks

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1qLqK0Tc4o4tVRUyx8hYxHka0pRaB0z_k)

This repository contains the complete implementation, training pipeline, evaluations, and competition model for **Project 1 (Cat & Dog Classification)** at the University of Southern Denmark (SDU), Fall 2026.

---

### Project Structure
* `First Project - Deep Learning.ipynb`: Complete self-contained Google Colab & Jupyter notebook covering:
  * **Task 1:** 70/15/15 stratified data split, PyTorch `Dataset`, and on-the-fly data augmentations (`RandomHorizontalFlip`, `RandomRotation`, `ColorJitter`).
  * **Task 2:** Parameter-efficient CNN (<100,000 parameters) using VGG-style $3\times3$ convolutions and **Global Average Pooling** (targeting the Cake Competition).
  * **Task 3:** Training vs. validation curves, test set confusion matrix, misclassified error analysis, and feature map visualizations.
  * **Competition Export:** Automatic generation and verification of `competition.py` and `competition.pth`.

---

### Dataset
The dataset consists of 2,400 RGB images (1,200 cats and 1,200 dogs).
* The dataset is attached as `catdog_data.zip` in [Release v1.0](https://github.com/johannm00-ux/Deep-Learning-Project-1/releases/tag/v1.0).
* The notebook automatically downloads and unzips the dataset directly to the Colab local SSD when executed.

---

### Teammates Collaboration
To open and run this project in Google Colab:
1. Open the notebook via Google Drive or [Google Colab Link](https://colab.research.google.com/drive/1qLqK0Tc4o4tVRUyx8hYxHka0pRaB0z_k).
2. Enable GPU acceleration: **Runtime $\rightarrow$ Change runtime type $\rightarrow$ T4 GPU**.
3. Run all cells sequentially.
