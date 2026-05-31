# 🛒 Supervised ML Model Comparison — Online Retail Dataset

> Implementing and comparing **Logistic Regression**, **Decision Tree**, and **K-Nearest Neighbors** classifiers on real-world retail purchase data.

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Objectives](#-objectives)
- [Dataset](#-dataset)
- [Technologies Used](#-technologies-used)
- [Project Workflow](#-project-workflow)
- [Machine Learning Models](#-machine-learning-models)
- [Evaluation Metrics](#-evaluation-metrics)
- [Results](#-results)
- [Future Improvements](#-future-improvements)
- [Learning Outcomes](#-learning-outcomes)
- [Conclusion](#-conclusion)

---

## 📖 Project Overview

This project implements and compares multiple supervised Machine Learning algorithms using an **Online Retail Dataset**. The goal is to analyze customer purchase data, perform preprocessing, train different classification models, evaluate their performance, and compare results through visualization.

---

## 🎯 Objectives

- Understand the complete Machine Learning workflow
- Perform data preprocessing and feature engineering
- Train multiple supervised learning models
- Evaluate model performance using standard metrics
- Compare algorithms and interpret results

---

## 📊 Dataset

| Property | Details |
|---|---|
| **Name** | Online Retail Dataset |
| **Source** | [Kaggle](https://www.kaggle.com) |
| **Features Used** | `Quantity`, `UnitPrice`, `Country` |
| **Target Variable** | `PurchaseType` (Binary) |

### 🎯 Target Variable — `PurchaseType`

The target is generated using the **median value of Quantity**:

| Label | Class | Description |
|---|---|---|
| `1` | High Purchase | Quantity ≥ median |
| `0` | Low Purchase | Quantity < median |

---

## 🛠️ Technologies Used

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

---

## 🔄 Project Workflow

```
📂 Load Dataset
      ↓
🔧 Data Preprocessing
   ├── Handle missing values
   ├── Select relevant features
   └── Encode categorical data (LabelEncoder)
      ↓
📊 Data Visualization
   ├── Customer Distribution Graph
   ├── Scatter Plot (Quantity vs UnitPrice)
   └── Model Accuracy Comparison Graph
      ↓
🤖 Model Training
   ├── Logistic Regression
   ├── Decision Tree Classifier
   └── K-Nearest Neighbors (KNN)
      ↓
📈 Model Evaluation
   ├── Accuracy Score
   └── Confusion Matrix
      ↓
📊 Model Comparison
```

---

## 🤖 Machine Learning Models

### 1. 📉 Logistic Regression
A linear model used for binary classification. It estimates the probability of a class using the sigmoid function.

### 2. 🌳 Decision Tree Classifier
A tree-based model that splits data based on feature thresholds. Easy to interpret and visualize.

### 3. 📍 K-Nearest Neighbors (KNN)
An instance-based learning algorithm that classifies data points based on the majority vote of the `k` nearest neighbors.

---

## 📏 Evaluation Metrics

### Accuracy Score
Measures the percentage of correctly classified instances.

$$\text{Accuracy} = \frac{TP + TN}{TP + TN + FP + FN}$$

### Confusion Matrix

|  | Predicted Positive | Predicted Negative |
|---|---|---|
| **Actual Positive** | TP (True Positive) | FN (False Negative) |
| **Actual Negative** | FP (False Positive) | TN (True Negative) |

---

## 📈 Results

| Model | Accuracy |
|---|---|
| 🔵 Logistic Regression | High |
| 🟢 Decision Tree | Very High |
| 🟡 K-Nearest Neighbors | High |

> ⚠️ **Note:** Actual results may vary depending on preprocessing steps, random state, and train-test split ratio.

---

## 🚀 Future Improvements

- [ ] Use additional features from the dataset
- [ ] Apply feature scaling (StandardScaler / MinMaxScaler)
- [ ] Perform hyperparameter tuning (GridSearchCV)
- [ ] Explore ensemble methods — **Random Forest**, **XGBoost**
- [ ] Use **cross-validation** for more robust evaluation
- [ ] Add ROC-AUC curve analysis

---

## 🧠 Learning Outcomes

After completing this project, you will understand:

✅ Data preprocessing techniques  
✅ Feature encoding methods  
✅ Supervised learning concepts  
✅ Model evaluation techniques  
✅ Accuracy and confusion matrix interpretation  
✅ Performance comparison of ML algorithms  

---

## ✅ Conclusion

This project demonstrates the implementation and comparison of **Logistic Regression**, **Decision Tree**, and **KNN** classifiers on an Online Retail Dataset. Through preprocessing, visualization, model training, and evaluation, the project highlights the importance of selecting suitable algorithms and evaluation metrics for classification tasks.

---

## 📁 Project Structure

```
📦 online-retail-ml/
├── 📄 README.md
├── 📓 notebook.ipynb
├── 📂 data/
│   └── online_retail.csv
├── 📂 plots/
│   ├── customer_distribution.png
│   ├── scatter_quantity_price.png
│   └── model_accuracy_comparison.png
└── 📂 models/
    ├── logistic_regression.py
    ├── decision_tree.py
    └── knn.py
```

---

<p align="center">
  Made with ❤️ using Python & Scikit-learn
</p>
