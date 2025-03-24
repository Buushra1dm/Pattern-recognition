# Water Safety Classification

## Project Overview
This project aims to design and implement a suitable pattern recognition technique to classify different water safety conditions. The focus is on leveraging machine learning models to determine whether a given water sample is safe or unsafe for consumption.

## Course
- CCAI312 - Pattern Recognition

## Problem Statement
Many communities, especially in Africa, struggle with access to clean and safe drinking water. This project seeks to address this issue by applying machine learning models to classify water samples based on various features, improving the efficiency of water safety assessment.

## Dataset
- The dataset contains **7999 rows (samples)** and **21 columns (features + class label)**.
- Some key challenges in the dataset include:
  - **Unbalanced data**
  - **Missing values**

## Methodology
### 1. Exploratory Data Analysis (EDA)
- Identified missing values and class distribution.
- Visualized key dataset properties.

### 2. Preprocessing
- Removed records with missing values (`NUM!`).
- Converted object-type columns to numerical data types.
- Normalized the dataset to ensure consistent feature scaling.
- Applied **random oversampling** to handle class imbalance.

### 3. Machine Learning Models
#### **Decision Tree**
- Selected due to its ability to handle both categorical and numerical data.
- Hyperparameter tuning results:
  - Criterion: `gini`
  - Max depth: `4`
  - Max features: `None`
  - Splitter: `best`
- **Strengths:**
  - Requires minimal computation
  - Handles missing values effectively
  - Suitable for large datasets
- **Weaknesses:**
  - Prone to overfitting
  - Can be unstable

#### **Support Vector Machine (SVM)**
- Used for classification by finding the best hyperplane to separate different classes.
- Key hyperparameters optimized:
  - **Kernel**
  - **C (Regularization parameter)**
  - **Gamma**
- **Strengths:**
  - Highly accurate
  - Can handle high-dimensional data
- **Weaknesses:**
  - Computationally expensive
  - Slow training time

## Results
- The **Decision Tree** model performed better on this dataset compared to **SVM** in terms of efficiency.
- The final model successfully classifies water safety, contributing to improved water quality assessment.

## Conclusion
This project demonstrates the effectiveness of machine learning techniques, particularly **Decision Trees**, in classifying water safety. Future improvements could include experimenting with **ensemble methods** like Random Forests and exploring **deep learning approaches** for more robust classification.

