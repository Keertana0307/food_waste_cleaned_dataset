# Food Waste Prediction Using Machine Learning Models

This repository contains the cleaned dataset and experimental notebooks for predicting food waste quantities using multiple machine learning and deep learning models. The study evaluates both traditional and advanced approaches, including a Knowledge-integrated Neural Network (KiNN), to assess their effectiveness in modelling food waste based on operational and environmental indicators.

The primary objective of this work is to compare model performance and analyse the suitability of different modelling techniques for food waste prediction.

---

## Repository Structure

food_waste_cleaned_dataset/
│
├── data/
│ └── cleaned_food_waste_dataset.xlsx
│
├── notebooks/
│ ├── 01_data_preprocessing.ipynb
│ ├── 02_baseline_models.ipynb
│ ├── 03_kinn_model.ipynb
│
└── README.md


- **data/**  
  Contains the cleaned dataset used for all experiments.

- **notebooks/**  
  Includes data preprocessing, baseline machine learning models, and the KiNN implementation.

---

## Models Implemented

The following models are evaluated in this study:

- XGBoost
- Random Fprest
- Feedforward Neural Network (FNN)
- Knowledge-integrated Neural Network (KiNN)

Model performance is assessed using standard regression metrics such as R², MAE, and RMSE.

---

## How to Run

1. Open any notebook directly in Google Colab.
2. Run all cells sequentially.  
The dataset is loaded directly from this GitHub repository; no local setup or Google Drive access is required.

---

## Dataset

The cleaned dataset contains food waste records with operational, environmental, and categorical attributes.  
All preprocessing steps (handling missing values, zero-value filtering, and feature standardisation) are documented in the preprocessing notebook.

---

## Dependencies

- Python 3.9+
- pandas
- numpy
- scikit-learn
- PyTorch

All dependencies are pre-installed in Google Colab.

---

## Academic Note

This repository is part of an academic project and is intended for reproducibility and methodological comparison rather than deployment.


