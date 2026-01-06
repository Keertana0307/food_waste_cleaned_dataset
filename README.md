# Food Waste Prediction Using Machine Learning Models

## Overview
This repository contains the cleaned dataset and source code used for predicting food waste in the United States using machine learning models. The study focuses on estimating the total amount of surplus food that becomes waste (`tons_waste`) by leveraging supply, consumption, environmental footprint, and contextual variables from the ReFED Food Waste Monitor dataset.

Four predictive models were implemented and compared:
- XGBoost  
- Random Forest  
- Feedforward Neural Network (FNN)  
- Knowledge-Integrated Neural Network (KiNN)

The objective is to evaluate model performance, identify key drivers of food waste, and support sustainability-oriented decision making.

---

## Dataset
The dataset used in this study is derived from the **ReFED Food Waste Monitor** and has undergone extensive preprocessing to ensure data quality and suitability for modelling.

**Key characteristics:**
- Final dataset size: **75,101 records**
- Target variable: `tons_waste`
- Numerical features include:
  - `tons_surplus`
  - `tons_uneaten`
  - `tons_supply`
  - `meals_wasted`
  - Environmental footprint variables (CO₂e, CH₄, water footprint)
- Categorical features include:
  - `state`
  - `sector`
  - `sub_sector`
  - `food_type`

The cleaned dataset is included in this repository for reproducibility.

---

## Repository Structure
This repository includes the following scripts and notebooks:

- **Data Preprocessing**
  - Column standardization and data type enforcement  
  - Feature selection  
  - Handling missing and zero values  
  - Outlier removal using 1st–99th percentile filtering  
  - Log transformation of the target variable  

- **Model Implementations**
  - XGBoost
  - Random Forest
  - Feedforward Neural Network (FNN)
  - Knowledge-Integrated Neural Network (KiNN)

Each model includes training, validation, and evaluation using standard regression metrics.

---

## Google Colab Notebook
All preprocessing and model training steps can be executed directly using Google Colab:

**Google Colab Link:**  
[https://colab.research.google.com/drive/1eoKg7vEWAQFmKNUdlKfc0a5XLtteKe_s](https://colab.research.google.com/drive/1eoKg7vEWAQFmKNUdlKfc0a5XLtteKe_s?usp=sharing)

The notebook provides an end-to-end workflow, including data loading, preprocessing, model training, and performance evaluation.

---

## Evaluation Strategy
Model performance is evaluated using:
- **R²** (coefficient of determination)
- **RMSE** (Root Mean Squared Error)
- **MAE** (Mean Absolute Error)

Five-fold cross-validation is applied to ensure robustness and generalizability of results.

---

## Key Findings
- Ensemble models (Random Forest and XGBoost) achieved the highest predictive accuracy.
- Random Forest performed best overall, with the lowest RMSE and MAE.
- Consumption-related variables such as `meals_wasted` and `tons_uneaten` were the most influential predictors.
- Neural network models were less effective on structured tabular data compared to ensemble models.

---

## Usage
1. Clone the repository  
2. Open the Google Colab notebook or run scripts locally  
3. Load the cleaned dataset  
4. Execute preprocessing and model training scripts  

---

## Data Source
ReFED Food Waste Monitor  
[https://insights-engine.refed.org/food-waste-monitor](https://insights-engine.refed.org/food-waste-monitor?view=overview&year=2023)
