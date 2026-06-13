# Fruit Image Classification Pipeline

## Overview

This repository contains a complete fruit image classification workflow incorporating image preprocessing, deep feature extraction using pretrained convolutional neural networks, and machine learning-based classification.

The pipeline supports automated dataset preparation, preprocessing, feature extraction, model training, evaluation, and result generation for banana and guava image datasets.

---

## Dataset

This project uses the **"Fruits (Banana and Guava) datasets for non-destructive quality classifications"** dataset published on **Mendeley Data**.

### Dataset Information

* **Title:** Fruits (Banana and Guava) datasets for non-destructive quality classifications
* **Version:** 2
* **Published:** 16 September 2024
* **DOI:** https://doi.org/10.17632/56td5w4wz2.2
* **Dataset Link:** https://data.mendeley.com/datasets/56td5w4wz2/2
* **Contributors:** Abiban Kumari and Jaswinder Singh

### Dataset Description

The dataset contains images of **banana** and **guava** fruits collected for non-destructive quality assessment and classification tasks. The images represent different quality categories and can be used for computer vision, machine learning, and deep learning applications related to fruit grading, quality inspection, and defect detection.

The dataset is automatically downloaded and organized during pipeline execution.

### Dataset Structure

```text
data/
│
├── raw/
│   ├── Banana/
│   │   ├── Class_A/
│   │   ├── Class_B/
│   │   └── Defect/
│   │
│   └── Guava/
│       ├── Class_A/
│       ├── Class_B/
│       └── Defect/
│
└── processed/
```

> Note: The exact class names and folder organization may vary slightly depending on the downloaded dataset version. The pipeline automatically organizes the images into the required directory structure for preprocessing and feature extraction.

---

## Repository Structure

```text
project/
│
├── src/
│   └── download_dataset.ipynb
│
├── notebooks/
│   ├── run_pipeline.ipynb
│   ├── final_preprocessing_pipeline.ipynb
│   └── reproducible_feature_extraction_pipeline.ipynb
│
├── data/
│
├── outputs/
│   ├── models/
│   ├── plots/
│   ├── reports/
│   ├── logs/
│   └── results/
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Feature Extraction Models

The pipeline supports deep feature extraction using the following pretrained convolutional neural networks:

* VGG16
* VGG19
* ResNet50
* MobileNet
* EfficientNetB0
* InceptionV3
* ResNet101

---

## Machine Learning Classifiers

Extracted deep features can be used with the following classifiers:

* Linear Support Vector Machine (Linear SVM)
* Quadratic Support Vector Machine
* Cubic Support Vector Machine
* Random Forest
* Logistic Regression

---

## Installation

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Pipeline

Open the master notebook:

```text
notebooks/run_pipeline.ipynb
```

Execute all cells:

```text
Kernel → Restart & Run All
```

The workflow automatically:

1. Downloads the dataset from Mendeley Data
2. Organizes the dataset into the required directory structure
3. Performs image preprocessing
4. Extracts deep features using pretrained CNN models
5. Trains machine learning classifiers
6. Evaluates model performance
7. Generates output files, reports, and visualizations

---

## Outputs

Generated outputs are stored in:

```text
outputs/
│
├── models/
├── plots/
├── reports/
├── logs/
└── results/
```

Output files include:

* Trained models
* Classification reports
* Confusion matrices
* ROC curves
* Performance metrics
* Benchmark result tables
* CSV summary files

---

## Requirements

* Python 3.10+
* Jupyter Notebook
* TensorFlow
* Scikit-learn
* OpenCV
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Joblib

All required packages are listed in `requirements.txt`.

---

## Citation

If you use this repository in your research, please cite both the dataset and the associated publication.

### Dataset Citation

Kumari, A., & Singh, J. (2024). *Fruits (Banana and Guava) datasets for non-destructive quality classifications* (Version 2). Mendeley Data.

**DOI:** https://doi.org/10.17632/56td5w4wz2.2

### Dataset URL

https://data.mendeley.com/datasets/56td5w4wz2/2

### Code Citation

Code DOI: [Insert Zenodo DOI]
