# 🍷 Wine Quality Classification with Random Forest  
This project demonstrates how to classify red wine quality using the **Random Forest Classifier**. The tutorial covers the entire pipeline from data preprocessing, feature selection, model building, hyperparameter tuning, and performance evaluation using classification metrics and visualizations.

---

## 🎯 **Objective**  
The goal of this project is to create a machine learning model capable of accurately predicting wine quality based on its chemical properties. The focus is on improving prediction accuracy through feature engineering, hyperparameter tuning, and model evaluation.

---

## 📂 **Dataset Overview**  
**Dataset:** Red Wine Quality Dataset (from UCI Machine Learning Repository)  
- **Samples:** 1599 red wine samples  
- **Features:** 12 numeric features representing chemical properties, such as:  
  - Fixed Acidity  
  - Volatile Acidity  
  - Citric Acid  
  - Residual Sugar  
  - Chlorides  
  - Free Sulfur Dioxide  
  - Total Sulfur Dioxide  
  - Density  
  - pH  
  - Sulphates  
  - Alcohol  
- **Target Classes:**  
  - 0 → Poor Quality Wine  
  - 1 → Good Quality Wine  

---

## 🏗️ **Model: Random Forest Classifier**  
Random Forest is an ensemble learning method that builds multiple decision trees and combines them to improve classification accuracy. The model reduces overfitting by averaging the predictions of individual trees.

### **Why Random Forest?**  
✅ High accuracy for structured data  
✅ Handles missing values automatically  
✅ Reduces variance by combining multiple models  
✅ Handles both classification and regression tasks  

### **Hyperparameters Used**  
| Parameter | Value | Description |
|-----------|-------|-------------|
| `n_estimators` | 200 | Number of decision trees |
| `max_depth` | None | Maximum depth of each tree |
| `min_samples_split` | 2 | Minimum number of samples to split a node |
| `min_samples_leaf` | 1 | Minimum number of samples in a leaf |
| `bootstrap` | True | Whether to use bootstrapping |

---

## 🚀 **Performance Metrics**  
The model was evaluated using key classification metrics:  

| Metric | Value |
|--------|-------|
| **Accuracy** | 0.82 |
| **Precision** | 0.84 |
| **Recall** | 0.81 |
| **F1-Score** | 0.82 |
| **ROC AUC** | 0.906 |

✅ **High ROC AUC Score** → The model shows strong discriminatory power between good and poor-quality wines.  

---

## 📊 **Results and Visualizations**  
### 1. **Confusion Matrix**  
Illustrates the number of correct vs. incorrect predictions:  
- **True Positives:** 139  
- **True Negatives:** 122  
- **False Positives:** 27  
- **False Negatives:** 32  

### 2. **ROC Curve**  
- ROC AUC Score: **0.906**  
- The curve shows high true positive rates with low false positive rates, indicating strong model performance.  

### 3. **Feature Importance**  
- The most influential features were:  
  - **Alcohol**  
  - **Sulphates**  
  - **Volatile Acidity**  
  - **Total Sulfur Dioxide**  

### 4. **Predicted Probability Distribution**  
- The model makes confident predictions with a clear separation between good and poor wine probabilities.  

### 5. **Correlation Heatmap**  
- Strong correlation between **alcohol** and wine quality was observed.  
- Negative correlation between **density** and wine quality.  

### 6. **Pairplot**  
- Displayed relationships between key features, showing visible patterns in acidity and alcohol content.  

---

## ⚙️ **How to Run the Code**  
### 1. **Clone the Repository**  
```bash
git clone https://github.com/your-username/wine-quality-classification.git
cd wine-quality-classification
# Wine-Quality-Tutorial
