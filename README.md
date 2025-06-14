# 📊 Customer Churn Prediction Project

This project analyzes customer churn using real-world telecom data.  
It explores feature patterns, performs data cleaning and preprocessing, and builds classification models to predict which customers are most likely to leave.

---

## 📁 Project Structure
  ```
  customer_churn_analysis/
│
├── notebooks/ # Step-by-step Jupyter notebooks
│ ├── 01_initial_exploration.ipynb
│ ├── 02_feature_exploration.ipynb
│ ├── 03_data_cleaning.ipynb
│ └── 04_modeling.ipynb
│
├── src/ # (Optional) modular Python scripts (not yet used)
│ ├── data_cleaning.py
│ ├── feature_engineering.py
│ └── modeling.py
│
├── data/ # Raw dataset
│ └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── venv/ or .venv/ # Python virtual environment
├── README.md # Project documentation
└── .gitignore # Git ignore rules

  ```

---

## 🔧 Tech Stack

- Python 3.10+
- Jupyter Notebook
- pandas, numpy
- seaborn, matplotlib
- scikit-learn
- xgboost

---

## 🔍 Project Highlights

- Performed exploratory data analysis (EDA) on churn behavior
- Identified key churn drivers such as:
  - Contract type (month-to-month vs. long-term)
  - Tenure (length of customer relationship)
  - Monthly charges
  - Payment method
- Cleaned and encoded dataset for machine learning
- Built and compared three classification models:
  - Logistic Regression
  - Random Forest
  - XGBoost (best performance)

---

## 🏆 Model Comparison

| Model               | Accuracy | Precision | Recall | F1 Score | AUC  |
|---------------------|----------|-----------|--------|----------|------|
| Logistic Regression | 0.803    | 0.682     | 0.585  | 0.630    | 0.841 |
| Random Forest       | 0.812    | 0.705     | 0.617  | 0.658    | 0.854 |
| **XGBoost**         | **0.825**| **0.724** | **0.641**| **0.680**| **0.867** |

✅ **XGBoost** was selected as the final model due to its superior performance in recall and AUC — important for catching high-risk churners.

---

## 🚀 How to Run This Project

1. Clone this repo:
   ```bash
   git clone https://github.com/yourusername/customer_churn_analysis.git
   cd customer_churn_analysis
2. Set up virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
3. Launch Jupyter:
   ```bash
   jupyter notebook
   
4. Open and run notebooks in order:
  
  01_initial_exploration → 02_feature_exploration → 03_data_cleaning → 04_modeling


## 📌 Future Improvements

-Refactor code into reusable .py modules (src/)

-Add dashboard (e.g. Streamlit) for interactive churn demo

-Hyperparameter tuning (GridSearchCV or Optuna)

-Model deployment as API or web app


## 🧑‍💻 Author
Jiawen Shen (Carmen)
📍 Calgary, Canada 
🎯 Aspiring Data Analyst
📧 carmenshun0629@gmail.com






