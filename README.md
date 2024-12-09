# Feature Store with ML Pipeline

## Overview

This project focuses on designing a **Feature Store** integrated with an ML pipeline using the `athletes.csv` dataset. The objective is to manage feature versions, run experiments with different configurations, and evaluate the results quantitatively and qualitatively. Additionally, the project includes an analysis of carbon emissions generated during model training.

---

## Objectives

1. Load and process data to create features with two distinct versions.
2. Set up a robust ML pipeline in an MLOps platform with feature store integration.
3. Train a machine learning algorithm using:
   - Two feature versions.
   - Two hyperparameter configurations for each feature version.
4. Compare model performance across configurations using metrics and plots.
5. Analyze the carbon emissions for each experiment.

---

## Dataset Details

### Source:  
`athletes.csv`

### Features:
- **Categorical Variables:** Include athlete metadata such as nationality, sport, and gender.
- **Numerical Variables:** Include performance statistics like height, weight, and age.

### Versions:
- **Feature Version 1:** Baseline features with minimal transformations.  
- **Feature Version 2:** Enhanced features with additional transformations and feature engineering.

---

## Methodology

### Data Preparation
1. **Data Loading:**  
   Load `athletes.csv` into a feature store. Handle missing values and preprocess features.

2. **Feature Engineering:**  
   Generate two versions of features:
   - **Version 1:** Basic cleaned dataset.  
   - **Version 2:** Includes additional engineered features (e.g., performance ratios, normalized stats).

---

### ML Pipeline
1. **MLOps Platform:**  
   Utilize an MLOps platform (Hopsworks/DagsHub) for pipeline automation and feature version management.

2. **Model Training:**  
   Train a machine learning model with:
   - Two feature versions.
   - Two hyperparameter sets for each feature version (total of four experiments).  

3. **Evaluation:**  
   - Quantitative metrics: RMSE, MAE, R².
   - Qualitative insights: Residual plots, feature importance visualizations.

---

### Experiment Tracking
- Track performance metrics and configurations for each experiment.
- Compare results across different feature versions and hyperparameter settings.

---

### Carbon Emissions
- Use [CodeCarbon](https://codecarbon.io) to measure emissions for each experiment.
- Compare the environmental impact of different configurations.

---

## Results

1. **Quantitative Analysis:**  
   - Metrics showed improved performance with enhanced feature engineering (Version 2).
   - Hyperparameter tuning significantly impacted model accuracy and efficiency.

2. **Qualitative Insights:**  
   - Visualizations revealed differences in feature importance between versions.  
   - Residual analysis highlighted areas of potential model improvement.

3. **Carbon Emissions:**  
   - Enhanced features and complex hyperparameter configurations increased emissions slightly.  
   - Trade-offs between accuracy and sustainability were documented.

---

## How to Use This Repository

### Clone the Repository:
```bash
git clone https://github.com/ArushiMakraria/feature-store-ml-pipeline
