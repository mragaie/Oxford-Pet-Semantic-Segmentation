# Semantic Segmentation Loss Functions Comparison

## DMET 1001 – Image Processing | Assignment 2

**German University in Cairo (GUC)**  
**Faculty of Media Engineering and Technology**  
**Spring 2026**

---

## Overview

This project investigates the effect of different loss functions on semantic segmentation performance.

A small **U-Net segmentation model** was trained using different loss functions and evaluated based on:

- Dice Score
- Intersection over Union (IoU)
- HD95 Boundary Metric

The goal is to compare region-based losses with boundary-aware losses and analyze their impact on segmentation accuracy and boundary quality.

---

## Dataset

**Dataset:** Oxford-IIIT Pet Dataset

The dataset contains images of 37 different pet breeds with corresponding trimap segmentation masks.

Dataset Link:
https://www.robots.ox.ac.uk/~vgg/data/pets/
