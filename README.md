# Predicting-Water-Quality-Index-in-Irish-Rivers-with-Explainable-Machine-Learning

# Predicting Water Quality Index in Irish Rivers with Explainable Machine Learning

## Overview

This project focuses on predicting the Water Quality Index (WQI) of Irish rivers using machine learning techniques and explainable artificial intelligence (XAI). The objective is to develop predictive models that can estimate river water quality based on environmental and water quality parameters while providing insights into the factors influencing the predictions.

The project utilizes a publicly available Irish Water Quality Monitoring dataset and compares the performance of multiple machine learning models for WQI prediction.

---

## Dataset

**Dataset Source:**

Water Quality Monitoring Dataset (Ireland)

Source: https://figshare.com/articles/dataset/Water_Quality_Monitoring_Dataset_Ireland_/25002131

The dataset contains water quality measurements collected from Irish rivers and monitoring stations. These measurements are used to predict the Water Quality Index (WQI), which serves as an indicator of overall water quality status.

---

## Project Objectives

* Predict Water Quality Index (WQI) values using machine learning models.
* Compare the performance of multiple regression algorithms.
* Build reusable machine learning pipelines.
* Improve model interpretability using explainable AI techniques.
* Identify the most influential factors affecting water quality predictions.

---

## Repository Contents

| File                        | Description                                                                                                                        |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| Fullcode.ipynb              | Complete implementation including data preprocessing, feature engineering, model training, evaluation, and explainability analysis |
| WQI Results on Dataset.xlsx | Model performance results and evaluation metrics                                                                                   |
| linear_pipeline.pkl         | Trained Linear Regression pipeline                                                                                                 |
| rf_pipeline.pkl             | Trained Random Forest Regression pipeline                                                                                          |
| xgb_pipeline.pkl            | Trained XGBoost Regression pipeline                                                                                                |

---

## Machine Learning Models

The following machine learning models were developed and evaluated:

1. Linear Regression
2. Random Forest Regressor
3. XGBoost Regressor

Each model was trained using a machine learning pipeline that includes preprocessing and prediction stages.

---

## Explainable AI

Explainability techniques were applied to understand model predictions and feature importance. These techniques help identify which environmental and water quality variables contribute most significantly to the predicted Water Quality Index.

Benefits of Explainable AI include:

* Improved transparency
* Better model interpretation
* Increased trust in predictions
* Identification of key water quality indicators

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/jenyokeke123-sketch/Predicting-Water-Quality-Index-in-Irish-Rivers-with-Explainable-Machine-Learning.git
```

### Install Dependencies

```bash
pip install pandas numpy scikit-learn xgboost shap matplotlib seaborn jupyter
```

---

## Running the Project

1. Download the dataset from the Figshare source.
2. Place the dataset in the project directory.
3. Open the notebook:

```bash
jupyter notebook Fullcode.ipynb
```

4. Execute all cells sequentially.

---

## Model Files

The trained models are stored as serialized pipeline files:

* linear_pipeline.pkl
* rf_pipeline.pkl
* xgb_pipeline.pkl

These models can be loaded directly for inference without retraining.

Example:

```python
import pickle

with open("rf_pipeline.pkl", "rb") as f:
    model = pickle.load(f)

prediction = model.predict(new_data)
```

---

## Results

The performance comparison of all trained models is provided in:

**WQI Results on Dataset.xlsx**

The results include evaluation metrics and comparative analysis of model accuracy and predictive capability.

---

## Applications

* River water quality monitoring
* Environmental assessment
* Water resource management
* Early detection of water quality deterioration
* Decision support for environmental agencies

---

## Future Work

* Integration of real-time sensor data
* Deployment as a web-based prediction system
* Advanced explainability methods
* Deep learning-based WQI prediction
* Geospatial analysis of water quality trends

---

## Author

Jeniffer

MSc Research Project

Predicting Water Quality Index in Irish Rivers with Explainable Machine Learning
