# Neuroblastoma Clinical Outcome Prediction using Machine Learning

## Overview
This repository presents a machine learning project focused on predicting missing clinical outcomes in neuroblastoma using RNA-seq data and patient metadata.

As part of a group MSc project in Bioinformatics, we explored how machine learning can support clinical prediction in incomplete biomedical datasets by leveraging gene expression profiles and clinical variables.

## Problem Statement
Neuroblastoma is a heterogeneous childhood cancer with variable clinical outcomes. Missing clinical information can limit downstream analysis, interpretation, and decision-making.

The goal of this project was to build and compare machine learning models capable of predicting missing clinical endpoints, including:
- Disease progression
- INSS tumour stage
- High-risk classification
- Mortality related to disease

## Dataset
The project used:
- RNA-seq gene expression data with approximately 23,146 genes
- Clinical metadata for 498 samples

Clinical features included variables such as:
- Age at diagnosis
- Sex
- INSS stage
- Disease progression
- High-risk status
- Death from disease

## Workflow
The project followed a structured data science pipeline:

1. Data exploration
2. Data cleaning and preprocessing
3. Missing data handling
4. Outlier detection
5. Standardization
6. Dimensionality reduction using PCA
7. Model training and comparison
8. Cross-validation and hyperparameter tuning
9. Interpretation of results

## Methods
We evaluated multiple machine learning models, including:
- Logistic Regression
- Support Vector Machine (SVM)
- K-Nearest Neighbours (KNN)
- Random Forest
- Neural Network

To improve generalization and reduce overfitting:
- PCA was applied to address the curse of dimensionality
- K-fold cross-validation was used for model validation
- Hyperparameter tuning was performed for model optimization

## Key Contributions
- Worked on a high-dimensional biomedical dataset combining RNA-seq and clinical data
- Applied preprocessing steps including matching sample identifiers, removing constant-value features, standardization, and outlier detection
- Used PCA to reduce dimensionality before model training
- Compared multiple machine learning algorithms for predicting missing clinical outcomes
- Evaluated models using accuracy, precision, recall, F1-score, and AUC

## Key Findings
- Logistic Regression showed the most robust and consistent overall performance across the evaluated clinical factors
- Simpler models can outperform more complex models in some biomedical prediction tasks
- Machine learning can support the estimation of missing clinical variables in cancer datasets when preprocessing and validation are handled carefully

## Project Visuals

### Workflow
![Workflow](images/workflow.png)

### Data Distribution
![Data Distribution](images/data_distribution.png)

### Correlation Matrix
![Correlation Matrix](images/correlation_matrix.png)

### Model Comparison
![Model Comparison](images/model_comparison.png)

## Tools and Technologies
- Python
- scikit-learn
- pandas
- NumPy
- matplotlib
- seaborn
- PCA
- K-fold cross-validation

## Limitations
- This was a group academic project based on a specific dataset
- Missingness mechanisms may affect model validity
- Results may not fully generalize to other datasets without external validation

## Future Improvements
- Test the models on external datasets
- Compare RNA-seq with microarray-based approaches
- Explore feature selection strategies for stronger interpretability
- Investigate treatment-related variables as additional predictors
- Extend the pipeline with explainability methods such as SHAP

## Contribution Note
This repository is based on a collaborative MSc group project. The work presented here reflects the overall project workflow and findings, with contributions shared across the team.

## Contact
If you are interested in bioinformatics, machine learning, or cancer genomics collaborations, feel free to connect with me on LinkedIn.
