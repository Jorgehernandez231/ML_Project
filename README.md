# ML_Project – End-to-End Machine Learning Pipeline

This repository contains an end-to-end machine learning workflow built in Jupyter Notebooks.  
The goal is to go from **raw data** to **a trained, evaluated model** following a clear, reproducible pipeline.

> 🔧 Tech stack: Python, Jupyter Notebook, pandas, NumPy, scikit-learn, matplotlib / seaborn

---

## 📂 Repository Structure

```text
ML_Project/
├── data/                  # Dataset(s) used in the project
│   └── <your_data_file>.csv
├── 1_EDA.ipynb            # Exploratory Data Analysis
├── 2_Preprocessing.ipynb  # Data cleaning & feature engineering
├── 3_Modeling.ipynb       # Model training, tuning & evaluation
└── .gitignore
🎯 Project Objective
The objective of this project is to build and evaluate a supervised machine learning model to:

Predict whether a client will subscribe to a term deposit (yes/no).

•Objective: Support marketing teams by prioritizing clients most likely to subscribe.
•Impact: Improve conversion rate and reduce campaign costs by targeting the right audience.

📊 Dataset
Source: Bank Marketing Dataset
(https://archive.ics.uci.edu/ml/datasets/bank+marketing) 

Client Information

age: Client’s age
job: Occupation type (admin, technician, management, services, etc.)
marital: Marital status (married, single, divorced)
education: Education level
default: Has credit in default (yes/no)
housing: Has a housing loan (yes/no)
loan: Has a personal loan (yes/no)

Campaign-related Information

contact: Communication channel used (cellular, telephone)
month: Month of last contact
day_of_week: Day of week of last contact
duration: Duration of last contact (in seconds)
campaign: Number of contacts during this campaign
pdays: Days since last contact in a previous campaign (-1 means no previous contact)
previous: Number of contacts before this campaign
poutcome: Outcome of previous marketing campaign

Target Variable

y: Did the client subscribe to a term deposit? (yes/no)


🔍 1. Exploratory Data Analysis (1_EDA.ipynb)
In this notebook, the data is explored to understand:

Shape of the dataset and basic statistics

Distribution of numerical and categorical variables

Missing values and data quality issues

Correlations between features

Relationship between features and the target

Typical visualizations used:

Histograms & boxplots for distributions

Bar charts for categorical features

Correlation heatmaps

Target vs feature plots (e.g. mean target rate by category)

🧹 2. Preprocessing & Feature Engineering (2_Preprocessing.ipynb)
This notebook prepares the data for modeling:

Handling missing values

Encoding categorical variables (e.g. One-Hot Encoding)

Scaling / standardizing numerical variables (if needed)

Creating new features (feature engineering), such as:

Aggregations / ratios

Binning / grouping

Flags (e.g. has_previous_contact, has_loan, etc.)

Train / test split

🤖 3. Modeling & Evaluation (3_Modeling.ipynb)
Here different models are trained and compared.

Logistic Regression

Random Forest

Gradient Boosting

XGBoost / other tree-based models

Typical steps:

Train baseline model

Use cross-validation to evaluate performance

Hyperparameter tuning (e.g. GridSearchCV or RandomizedSearchCV)

Compare models using metrics like:

Classification: Accuracy, Precision, Recall, F1, ROC-AUC

Regression: MAE, RMSE, R²

Inspect:

Confusion matrix and ROC curve (classification)

Feature importances / coefficients

Business interpretation of results
