# Fetal Health Classification 🚼🩺

## Introduction
This project leverages Cardiotocogram (CTG) data to classify fetal health into three categories:
- **Normal**
- **Suspect**
- **Pathological**

The goal is to assist in early detection and intervention for fetal health issues.

## Dataset
- **Source**: [Kaggle: Fetal Health Classification](https://www.kaggle.com/datasets/andrewmvd/fetal-health-classification)
- **Features**: The dataset includes various features such as:
  - Baseline FHR (Fetal Heart Rate)
  - Accelerations
  - Decelerations
  - Uterine contractions
  - And more...

## Methodology
1. **Exploratory Data Analysis (EDA)**:
   - Visualized feature distributions and relationships.
   - Identified outliers and patterns in the data.

2. **Data Preprocessing**:
   - Applied Winsorization to handle outliers.
   - Standardized features using `StandardScaler`.

3. **Handling Imbalance**:
   - Used SMOTE (Synthetic Minority Oversampling Technique) strictly after splitting the data into training and testing sets.

4. **Dimensionality Reduction**:
   - Performed Principal Component Analysis (PCA) to reduce dimensionality and improve model performance.

## Models Used
### Classification:
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)
- XGBoost

### Regression:
- Linear Regression
- Random Forest Regressor

## Results
- **Random Forest** and **XGBoost** achieved the best classification performance with an accuracy of approximately **94-97%**.

## Interpretability
- **SHAP Values**: Used to explain the contribution of each feature to the model's predictions.
- **LIME Analysis**: Provided local interpretability for individual predictions.

## Installation
To set up the project, install the required dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn shap lime
```

## Author
Aleksandra Djokic 2145