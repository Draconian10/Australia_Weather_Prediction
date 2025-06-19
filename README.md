# Australia Weather Prediction

**Forecasting Rainfall in Australia Using Machine Learning**

This repository presents a comprehensive and well-structured machine learning pipeline designed to address the binary classification problem of predicting "Will it rain tomorrow?" based on historical weather data from various locations across Australia. Leveraging real-world meteorological features such as humidity, temperature, wind speed, atmospheric pressure, and more, this project builds predictive models that aim to deliver actionable weather insights.

The workflow encompasses the entire data science lifecycle, beginning with data exploration, cleaning, and feature engineering, followed by the development and evaluation of several machine learning models including Logistic Regression, LightGBM, and AutoML frameworks like PyCaret and H2O AutoML. Beyond model performance, the project places a strong emphasis on model transparency and interpretability using state-of-the-art techniques such as SHAP (SHapley Additive Explanations), LIME (Local Interpretable Model-agnostic Explanations), and Partial Dependence Plots (PDPs).

Together, these components form a replicable and educational pipeline suitable for both practitioners and learners looking to understand not just how to build machine learning models, but also how to interpret and trust their predictions in real-world decision-making contexts.

---

## 📚 Project Overview

* **Problem**: Predict rainfall the next day based on past weather observations.
* **Data**: Historical weather data from multiple Australian weather stations.
* **Models Used**: Logistic Regression, LightGBM, PyCaret AutoML, H2O AutoML.
* **Techniques Covered**:

  * Data cleaning & imputation (Simple, Median, MICE)
  * Feature engineering and selection
  * Model training & evaluation
  * Model explainability (SHAP, LIME, PDP)

---

## 📦 Dataset

* **Source**: [Kaggle - Australia Weather Dataset](https://www.kaggle.com/datasets/arunavakrchakraborty/australia-weather-data)
* **Format**: CSV (`Weather Training Data.csv`)
* **Note**: Please download the dataset from Kaggle and place it in the appropriate folder before executing notebooks.

---

## 🗂️ Repository Structure

```text
Australia_Weather_Prediction/
├── Combined_Report.ipynb
├── AutoML/
│   └── AutoML_PyCaret.ipynb
├── Data_Cleaning_Feature_Selection/
│   ├── ML_Data_Cleaning_Feature_Selection.ipynb
│   └── Weather Training Data.csv
├── Model_Interpretability/
│   └── Model_Interpretability.ipynb
├── LICENSE
└── README.md
```

---

## 📘 Notebooks Breakdown

### 📌 `Combined_Report.ipynb`

A unified notebook that integrates:

* Data cleaning & imputation
* Feature selection & correlation analysis
* Model training: Logistic Regression, LightGBM, H2O AutoML
* Evaluation metrics & model explainability
* SHAP, LIME, and PDP visualizations

> Recommended for users who prefer an end-to-end overview in one place.

---

### 🧼 `Data_Cleaning_Feature_Selection/ML_Data_Cleaning_Feature_Selection.ipynb`

Focuses on robust preprocessing and feature engineering:

* Exploratory Data Analysis (EDA)
* Imputation strategies: Simple, Median, Most Frequent, MICE
* Outlier detection & effect on model performance
* Feature scaling, correlation analysis, and selection
* Pre-modeling insights and hypothesis testing

---

### 🤖 `AutoML/AutoML_PyCaret.ipynb`

An AutoML pipeline using PyCaret for classification tasks:

* Minimal-code model setup and training
* Model comparison, tuning, and evaluation
* SHAP-based feature importance
* AUC and prediction analysis
* Regularization (Ridge/Lasso) and assumption validation

> Best for quick prototyping and AutoML experimentation.

---

### 📊 `Model_Interpretability/Model_Interpretability.ipynb`

Dedicated to model explainability:

* SHAP, LIME, and PDP visualizations
* Comparative interpretability across models (Logistic, LightGBM, H2O)
* Evaluation of assumptions and insights drawn from interpretation methods

> Ideal for data scientists focused on model transparency.

---

## 📈 Models Implemented

| Model               | Framework    | Interpretability Tools |
| ------------------- | ------------ | ---------------------- |
| Logistic Regression | scikit-learn | SHAP, LIME, PDP        |
| LightGBM            | LightGBM     | SHAP, LIME, PDP        |
| PyCaret AutoML      | PyCaret      | Built-in + SHAP        |
| H2O AutoML          | H2O.ai       | SHAP, PDP              |

---

## 🛠️ Installation & Setup

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Draconian10/Australia_Weather_Prediction.git
   cd Australia_Weather_Prediction
   ```

2. **Install Required Packages**

   ```bash
   pip install -r requirements.txt
   ```

3. **Start Jupyter**

   ```bash
   jupyter notebook
   ```

---

## 📌 Key Highlights

* ✔️ Multiple Imputation Methods Compared
* ✔️ End-to-End ML Workflow
* ✔️ Powerful Explainability Techniques
* ✔️ AutoML with H2O and PyCaret
* ✔️ Interpretation-Driven Conclusions
