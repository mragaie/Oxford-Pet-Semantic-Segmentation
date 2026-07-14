# DMET1001 - Assignment 2: Semantic Segmentation

## Team Information

| Name | ID | Tutorial |
|------|------|------|
| Youssef Khaled | 55-0814 | T-09 |
| Omar Ayman | 55-7986 | T-10 |
| Mohamed Elnaggar | 55-1745 | T-10 |
| Malak Ragaie | 55-25294 | T-10 |

---

## Project Overview

This project investigates the effect of different segmentation loss functions on semantic segmentation performance using a U-Net architecture.

The following models were trained and compared:

- Model A: Dice Loss
- Model B: Hausdorff-inspired Loss
- Model C: Tversky Loss
- Model D: Combined Loss

Evaluation metrics:

- Dice Score
- Intersection over Union (IoU)
- HD95

---

## Dataset

Dataset used:

- [Oxford-IIIT Pet Dataset]

Dataset split:

- Training: 70%
- Validation: 15%
- Testing: 15%

Random seed used:

```python
seed = 42
```

# Execution Instructions

## 1. Required Libraries

The project was implemented using PyTorch in Kaggle Notebooks.

Required libraries:

```bash
pip install torch torchvision numpy matplotlib pillow scipy scikit-image
```

---

## 2. Running the Project

The notebook was developed and executed using Kaggle Notebook GPU acceleration.

To run the project:

1. Upload the notebook file to Kaggle.
2. Enable GPU acceleration from the notebook settings.
3. Run all notebook cells sequentially from top to bottom.

The notebook automatically performs:

- Dataset download and preprocessing
- Distance transform generation
- U-Net model construction
- Loss function implementation:
  - Dice Loss
  - Hausdorff-inspired Loss
  - Tversky Loss
  - Combined Loss
- Training of all four models
- Evaluation using Dice Score, IoU, and HD95
- Visualization and comparison plot generation

---

## 3. Trained Model Weights

Saved model weights are included inside:

```text
model_weights/
```

Example files:

```text
model_A_dice.pth
model_B_hd95.pth
model_C_tversky.pth
model_D_combined.pth
```

---

## 4. Generated Outputs

The project generates:

- Training loss curves
- Dice score curves
- (IoU / HD95 / Dice score) quantitative comparison plots
- Visual comparison: Input | Ground Truth | Predictions
- Segmentation Overlays: Ground Truth | Prediction | Overlap

All generated figures are stored inside:

```text
plots/
```

---

## 5. Hardware

The project was trained using Kaggle Notebook GPU acceleration.

Example environment:

```text
GPU T4 x2
```