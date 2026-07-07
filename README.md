# 📊 Risk Management on Granular Data

A machine learning project that predicts customer risk levels from transactional retail data using **CatBoost**, **Random Forest**, and an **Artificial Neural Network (ANN)**. The project combines customer behavior analytics, feature engineering, and explainable AI to identify high-risk customers from granular purchase records.

---

## 🚀 Project Overview

Understanding customer purchasing behavior is essential for improving customer retention, reducing business risk, and supporting data-driven decision-making.

This project analyzes transactional retail data to classify customers into **Low**, **Medium**, and **High** risk categories using machine learning. It follows a complete data science pipeline—from preprocessing and exploratory data analysis to feature engineering, model training, evaluation, and explainability.

---

## ✨ Features

* 📊 Exploratory Data Analysis (EDA)
* 🧹 Data cleaning and preprocessing
* 💰 RFM (Recency, Frequency, Monetary) analysis
* ⚙️ Customer-level feature engineering
* 🤖 CatBoost multiclass classification
* 🌲 Random Forest implementation
* 🧠 Artificial Neural Network (ANN)
* 📈 Model performance comparison
* 📉 ROC-AUC analysis
* 🎯 Precision, Recall, and F1-score evaluation

---

## 🛠️ Tech Stack

| Technology         | Purpose                      |
| ------------------ | ---------------------------- |
| Python             | Programming Language         |
| Google Colab       | Development Environment      |
| Pandas             | Data Processing              |
| NumPy              | Numerical Computing          |
| Matplotlib         | Data Visualization           |
| Scikit-learn       | Machine Learning Utilities   |
| CatBoost           | Gradient Boosting Classifier |
| TensorFlow / Keras | Artificial Neural Network    |
| SHAP               | Explainable AI               |

---

## 📂 Repository Structure

```text
Risk-Management-On-Granular-Data/
│
├── Catboost Risk Management.ipynb
├── README.md
```

---

## 📊 Dataset

The project uses a transactional retail dataset, the **Online Retail** dataset from the UCI Machine Learning Repository, containing customer purchase information, including:

* Invoice Number
* Invoice Date
* Customer ID
* Country
* Stock Code
* Product Description
* Quantity
* Unit Price

From these records, customer-level behavioral features are generated for risk prediction.

**Dataset Citation**

Chen, D. (2015). *Online Retail* [Dataset]. UCI Machine Learning Repository.
DOI: 10.24432/C5BW33

Dataset: https://archive.ics.uci.edu/dataset/352/online+retail

---

## 🔬 Project Workflow

### 1. Data Preprocessing

* Missing value handling
* Duplicate removal
* Datetime conversion
* Deal Value computation
* Outlier clipping

---

### 2. Exploratory Data Analysis

The notebook includes visualizations for:

* Top purchasing countries
* Monthly sales trends
* Most purchased products
* Customer purchasing behaviour

---

### 3. Feature Engineering

Features generated include:

* Deal Value
* Customer Frequency
* Product Frequency
* Invoice Month
* Invoice Day of Week
* Invoice Hour
* RFM Features

  * Recency
  * Frequency
  * Monetary

---

### 4. Risk Label Generation

Customers are segmented into:

* 🟢 Low Risk
* 🟡 Medium Risk
* 🔴 High Risk

using weighted RFM scoring.

---

### 5. Machine Learning Models

The project compares multiple approaches:

* ✅ CatBoost Classifier
* 🌲 Random Forest
* 🧠 Artificial Neural Network (ANN)

---

## 📈 Results

| Model         |  Accuracy |
| ------------- | --------: |
| CatBoost      | **90.5%** |
| Random Forest |     83.4% |
| ANN           |     79.2% |

### ROC-AUC

| Model         |      AUC |
| ------------- | -------: |
| CatBoost      | **0.94** |
| Random Forest |     0.88 |
| ANN           |     0.84 |

The CatBoost model achieved the highest overall performance, outperforming both Random Forest and the ANN across multiple evaluation metrics.

---

## 📊 Model Evaluation

The notebook evaluates models using:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC
* Classification Report

Performance comparisons are presented through charts and visualizations.

---

## 🔍 Explainability

To improve model interpretability, the project uses **SHAP (SHapley Additive exPlanations)** to identify the most influential features contributing to customer risk predictions.

---

## ▶️ Running the Project

Clone the repository:

```bash
1. Clone this repository: git clone https://github.com/Prasuk-2003/Risk-Management-On-Granular-Data.git
```

```bash
2. Download the Online Retail dataset from the UCI Machine Learning Repository.
```

```bash
3. Place the dataset in the project directory and accordingly change the code
   df = pd.read_excel('/content/Online Retail 3.xlsx').
```
```bash
4. Open the notebook in Google Colab or Jupyter Notebook.
```
```bash
5. Run the notebook cells sequentially.
```

---

## 📚 Concepts Demonstrated

* Machine Learning
* Feature Engineering
* Customer Segmentation
* RFM Analysis
* Ensemble Learning
* Neural Networks
* Explainable AI
* Model Evaluation
* Business Analytics

---

## 👨‍💻 Author

**Prasuk Minda**

GitHub: https://github.com/Prasuk-2003

---

## 📄 License

This project is intended for educational and research purposes.
