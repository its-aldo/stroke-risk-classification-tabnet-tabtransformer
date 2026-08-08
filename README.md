# Stroke Risk Classification Using TabNet and TabTransformer

This repository contains the implementation of an undergraduate thesis research on **stroke risk classification using tabular healthcare data**. The research compares the performance of **TabNet** and **TabTransformer** using Stratified K-Fold Cross Validation.

## Research Objective

The objective of this research is to evaluate and compare the performance of TabNet and TabTransformer in classifying stroke risk based on tabular healthcare data.

## Dataset

The dataset contains demographic, lifestyle, and medical-related attributes, including:

* Gender
* Age
* Hypertension
* Heart Disease
* Ever Married
* Work Type
* Residence Type
* Smoking Status
* Average Glucose Level
* BMI

The target variable is `stroke`, which represents whether an individual has experienced a stroke.

The dataset is not included in this repository.

## Methodology

The research process includes:

1. Data preprocessing
2. Handling missing values
3. Encoding categorical variables
4. Handling class imbalance using SMOTE
5. Feature scaling
6. Model training
7. Stratified K-Fold Cross Validation
8. Model evaluation
9. Comparison of TabNet and TabTransformer

## Models

### TabNet

TabNet is a deep learning architecture designed for tabular data. It uses sequential attention to select relevant features during the decision-making process.

### TabTransformer

TabTransformer is a Transformer-based architecture designed for tabular data. It uses self-attention mechanisms to learn contextual representations of categorical features.

## Cross Validation

Two validation scenarios were implemented:

* **5-Fold Cross Validation**
* **10-Fold Cross Validation**

Stratified K-Fold Cross Validation was used to preserve the class distribution in each fold.

## Repository Contents

```text
stroke-risk-classification-tabnet-tabtransformer/
│
├── k5_skripsi.ipynb
├── k10_skripsi.ipynb
└── README.md
```

### `k5_skripsi.ipynb`

Contains the complete implementation and evaluation of the TabNet and TabTransformer models using **5-Fold Stratified Cross Validation**.

### `k10_skripsi.ipynb`

Contains the complete implementation and evaluation of the TabNet and TabTransformer models using **10-Fold Stratified Cross Validation**.

## Evaluation Metrics

The models are evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC
* Confusion Matrix

These metrics are used to compare the classification performance of TabNet and TabTransformer.

## Main Results

The experimental results indicate that **TabNet achieved better overall performance than TabTransformer** based on Accuracy, Precision, F1-Score, and ROC-AUC.

TabTransformer, however, achieved higher Recall, indicating better sensitivity in identifying positive stroke cases.

## How to Run

1. Clone or download this repository.
2. Open either `k5_skripsi.ipynb` or `k10_skripsi.ipynb` using Jupyter Notebook, JupyterLab, or Google Colab.
3. Make sure the required Python libraries are installed.
4. Run the notebook cells sequentially.

The notebooks contain the preprocessing, model training, cross-validation, and evaluation processes.

## Requirements

The implementation uses Python and several machine learning and deep learning libraries, including:

* NumPy
* Pandas
* Scikit-learn
* PyTorch
* PyTorch TabNet
* imbalanced-learn
* Matplotlib
* Seaborn

## Disclaimer

This project was developed for academic and research purposes. The resulting models are **not intended for clinical diagnosis or medical decision-making**.

## Author

**Aldo Pratama**

Undergraduate Thesis Research
2026
