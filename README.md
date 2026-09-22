# CSC2042S Assignment 2

## Multinomial Logistic Regression for News Topic Classification

**Name:** Sanele Hopewell Nkosi  
**Student number:** nkssan033

## Overview

This project implements multinomial logistic regression for multilingual news topic classification using PyTorch.

The model is evaluated on the MasakhaNEWS datasets for:

- English
- isiXhosa
- chiShona

The project compares three text feature representations:

- Bag-of-Words
- Binary word presence
- TF-IDF

The experiments include:

- Text preprocessing
- Multinomial logistic regression
- Feature representation comparison
- Hyperparameter tuning
- Model weight analysis
- isiXhosa class-imbalance experiments
- Bilingual training
- Final test-set evaluation
- Confusion matrices
- Micro- and macro-averaged evaluation metrics

## Repository Contents

### `CSC2042S_Assignment_2.ipynb`

The main Jupyter notebook containing all assignment code and outputs.

The notebook includes:

1. Dataset loading and preprocessing
2. Feature extraction
3. Multinomial logistic regression implementation
4. Mini-batch model training
5. Hyperparameter tuning
6. Feature-weight analysis
7. isiXhosa upsampling and downsampling
8. Bilingual model training
9. Final model evaluation
10. Reproducibility and code-quality checks

### `CSC2042S_Assignment_2_Final_Report.tex`

The LaTeX source code for the assignment report.

### `CSC2042S_Assignment_2_Final_Report.pdf`

The compiled assignment report containing the experimental procedure, results, visualisations, and discussion.

### `validation_loss_curve.png`

The training and development loss curve for the development-selected isiXhosa Binary model. This image is included in the LaTeX report.

### `.gitignore`

Specifies files and folders that should not be tracked by Git, including dataset folders, notebook checkpoints, and temporary LaTeX build files.

## Dataset Structure

The MasakhaNEWS data must be stored using the following directory structure:

```text
CSC2042S-Assignment-2/
├── eng/
│   ├── train.tsv
│   ├── dev.tsv
│   └── test.tsv
├── xho/
│   ├── train.tsv
│   ├── dev.tsv
│   └── test.tsv
├── sna/
│   ├── train.tsv
│   ├── dev.tsv
│   └── test.tsv
├── CSC2042S_Assignment_2.ipynb
├── CSC2042S_Assignment_2_Final_Report.tex
├── CSC2042S_Assignment_2_Final_Report.pdf
├── validation_loss_curve.png
├── README.md
└── .gitignore