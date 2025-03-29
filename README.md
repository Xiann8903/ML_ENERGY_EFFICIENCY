# Energy Efficiency Prediction in Building Design

## 🔍 Problem Statement

The aim of this project is to develop a predictive model that can estimate the energy efficiency of buildings based on their architectural and design characteristics. The objective is to predict energy consumption metrics such as heating and cooling loads, which are critical for designing energy-efficient residential and commercial buildings.

This work is especially useful for architects, engineers, and sustainability professionals who want to assess and optimize building performance in early design phases using data-driven approaches.

## 🧠 Approach

The project follows a supervised machine learning pipeline and compares traditional ML models with deep learning techniques. The key steps include:

1. **Data Collection**: Load the dataset and inspect its structure.
2. **Data Preprocessing**: Handle missing values (if any), normalize features, and prepare inputs for modeling.
3. **Exploratory Data Analysis (EDA)**: Visualize feature distributions and analyze their correlation with energy loads.
4. **Model Development**:
   - Train a baseline model using Random Forest Regressor.
   - Build a Multi-Layer Perceptron (MLP) neural network with up to 3 hidden layers.
5. **Hyperparameter Tuning**:
   - Perform grid search to optimize model configurations.
6. **Evaluation**:
   - Compare model performance using RMSE (Root Mean Squared Error).
   - Plot and analyze predictions vs. actual values.
7. **Conclusion**: Summarize findings and provide recommendations for energy-efficient building design.

## 📊 Dataset

The dataset used in this project is called **`energy_efficiency_data`**, and it is available on **Kaggle**:

- **Source**: [Energy Efficiency Dataset on Kaggle](https://www.kaggle.com/datasets/amirhosseinmirzaie/energy-efficiency)

### 📦 Dataset Overview

This dataset contains simulation data from the Ecotect software, representing 768 building models with variations in shape, orientation, glazing, and other structural features. Each row corresponds to a different building configuration.

#### 🔧 Features:
- **Relative Compactness**
- **Surface Area**
- **Wall Area**
- **Roof Area**
- **Overall Height**
- **Orientation** (categorical: 2–5)
- **Glazing Area**
- **Glazing Area Distribution** (categorical: 0–5)

#### 🎯 Targets:
- **Heating Load (Y1)**: Energy required to heat the building (kWh/m²)
- **Cooling Load (Y2)**: Energy required to cool the building (kWh/m²)

The dataset focuses on how these building characteristics influence the energy demand for heating and cooling, and it supports regression-based modeling.

## 🛠 Technologies Used

- Python 3
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

## 📈 Evaluation Metric

The primary metric used to evaluate model performance is **Root Mean Squared Error (RMSE)**, which measures the average magnitude of prediction errors and penalizes larger deviations more strongly.

---

