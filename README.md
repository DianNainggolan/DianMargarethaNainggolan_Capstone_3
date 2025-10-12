# 📊 Customer Churn Prediction Project

## 🧭 Project Overview

Customer churn is a major challenge for many companies, especially in subscription and telecommunications industries. This project focuses on **analyzing and predicting customer churn** using **Exploratory Data Analysis (EDA)**, **data preprocessing**, and **machine learning techniques**.

By building a reliable churn prediction model, companies can **identify customers at risk of leaving** and take **timely actions** to improve retention and optimize revenue.

---

## 🎯 Project Objectives

* Analyze characteristics of churn vs non-churn customers.
* Identify variables that strongly influence churn.
* Build classification models to predict churn probability.
* Evaluate model performance and provide data-driven recommendations.
* Deliver actionable insights for business and marketing teams.

---

## 🧰 Technology and Libraries

This project uses Python and popular data science libraries:

| Category                 | Library / Tools                                   | Purpose                                        |
| ------------------------ | ------------------------------------------------- | ---------------------------------------------- |
| Data Processing          | `numpy`, `pandas`                                 | Data manipulation, aggregation, transformation |
| Data Visualization       | `matplotlib`, `seaborn`                           | EDA and churn pattern visualization            |
| Machine Learning         | `scikit-learn`, `xgboost`, `lightgbm`, `catboost` | Classification modeling and evaluation         |
| Statistics & Analysis    | `scipy`, `statsmodels`                            | Statistical analysis and hypothesis testing    |
| Imbalanced Data Handling | `imbalanced-learn`                                | Oversampling (SMOTE, SMOTEENN, SMOTETomek)     |
| Model Interpretability   | `shap`                                            | Model explanation using SHAP values            |
| Utility                  | `gdown`, `pickle`, `pathlib`                      | File download, model serialization             |
| Notebook Environment     | `jupyter`, `ipykernel`                            | Interactive experimentation                    |

---

## 📂 Project Structure

```
.
├── CapstoneProject_Module3_Dian Maragretha Nainggolan.ipynb   # Main notebook
├── data/                                                      # Dataset folder
│   └── customer_churn.csv
├── best_classifier_QDA.pkl
├── README.md
└── requirements.txt
```

---

## 📊 Project Workflow

### 1. Data Understanding

* Explore dataset structure and customer attributes.
* Identify numerical and categorical variables (tenure, contract, payment method, etc.).
* Analyze churn vs non-churn proportions.

### 2. Exploratory Data Analysis (EDA)

* Descriptive statistics and feature distributions.
* Churn visualization by customer segments.
* Correlation analysis between features and churn.
* Statistical tests (t-test, chi-square) to find significant drivers.

### 3. Data Preprocessing

* Handle duplicates.
* Encode categorical variables (OneHotEncoder, LabelEncoder).
* Normalize numeric features using `StandardScaler`.
* Split data into training and testing sets.
* Address class imbalance using:

  * RandomOverSampler
  * SMOTE
  * SMOTEENN
  * SMOTETomek

### 4. Modeling

Models tested:

* Logistic Regression
* Decision Tree
* Random Forest
* K-Nearest Neighbors
* Support Vector Machine
* Linear and Quadratic Discriminant Analysis (LDA & QDA)
* Gradient Boosting (XGBoost, LightGBM, CatBoost)

Hyperparameter tuning was performed using `GridSearchCV` or optimal defaults.

### 5. Model Evaluation

Evaluation metrics:

* Accuracy
* Precision, Recall, F1-Score
* ROC AUC
* Confusion Matrix

Boosting models (e.g., XGBoost / LightGBM) achieved the best performance with clear feature importance interpretation.

### 6. Model Interpretability

Using `shap`:

* Identify key features influencing churn probability.
* Provide actionable insights for business decisions.

### 7. Business Insights & Recommendations

* **Low tenure** and **monthly contracts** correlate with higher churn.
* **Automatic electronic payments** are linked to lower churn.
* Customers with **high monthly charges** are more likely to churn.
* High-risk segments may benefit from loyalty programs, promotions, or long-term contracts.

---

## 🧪 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/username/customer-churn-prediction.git
cd customer-churn-prediction
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```
CapstoneProject_Module3_Dian Maragretha Nainggolan.ipynb
```

### 4. Run All Cells

This will:

* Display data analysis
* Train machine learning models
* Evaluate performance
* Show model interpretability results

---

## 📝 requirements.txt

```
catboost
gdown
imbalanced-learn
ipykernel
jupyter
lightgbm
matplotlib
numpy
pandas
scikit-learn
scipy
seaborn
shap
xgboost
```

---

## 📈 Key Results

* Best ROC AUC Score: **> 0.85** (boosting models).
* Most influential features: tenure, contract type, monthly charges.
* Segmented churn insights enable targeted retention strategies.

---

## 🚀 Future Development

* Deploy model with Flask or Streamlit.
* Build an interactive business dashboard.
* Integrate real-time data for dynamic predictions.
* Connect with CRM systems for automated retention actions.

---

## 👩‍💻 Contributor

* **Dian Maragretha Nainggolan**
  Data Analyst | Machine Learning Enthusiast

---

## 📜 License

This project was created for learning and research purposes. Not for commercial distribution without written permission from the author.
