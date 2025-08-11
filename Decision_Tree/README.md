# 📊 Bank Marketing Client Subscription Prediction

## 📌 Overview
This project uses the **Bank Marketing Dataset** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing) to predict whether a client will subscribe to a term deposit (`y`: yes/no).  
We experiment with multiple classification algorithms — **Decision Tree**, **Random Forest**, **XGBoost**, and **AdaBoost** — and compare their performance.

---

## 🎯 Objective
- Predict **client subscription** outcome based on demographic, financial, and marketing interaction data.
- Compare performance of multiple ML algorithms.
- Evaluate models using metrics that are robust to class imbalance.

---

## 📂 Dataset
**Source:** UCI Bank Marketing Dataset  

**Key Features:**
- **Demographic**: `age`, `job`, `marital`, `education`
- **Financial**: `default`, `housing`, `loan`
- **Campaign-related**: `contact`, `month`, `day_of_week`, `duration`, `campaign`, `pdays`, `previous`, `poutcome`
- **Economic Indicators**: `emp.var.rate`, `cons.price.idx`, `cons.conf.idx`, `euribor3m`, `nr.employed`
- **Target Variable**: `y` (yes/no)

---

## 🛠️ Preprocessing
1. **Data Cleaning**
   - Removed missing/unknown values.
2. **Encoding**
   - Used **One-Hot Encoding** for categorical features.
3. **Train-Test Split**
   - 80% train / 20% test.

---

## 🤖 Models Used
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **XGBoost Classifier**
- **AdaBoost Classifier**

---

## 📊 Model Performance

### Decision Tree
- **Accuracy**: 0.89
- **Precision (True class)**: 0.53
- **Recall (True class)**: 0.54
- **F1-Score (True class)**: 0.54
- **ROC-AUC**: 0.7410

### Random Forest
- **Accuracy**: 0.92
- **Precision (True class)**: 0.67
- **Recall (True class)**: 0.49
- **F1-Score (True class)**: 0.56
- **ROC-AUC**: 0.9474

### XGBoost
- **Accuracy**: 0.92
- **Precision (True class)**: 0.69
- **Recall (True class)**: 0.56
- **F1-Score (True class)**: 0.62
- **ROC-AUC**: 0.9546

### AdaBoost
- **Accuracy**: 0.90
- **Precision (True class)**: 0.72
- **Recall (True class)**: 0.25
- **F1-Score (True class)**: 0.38
- **ROC-AUC**: 0.9366

---

## 📈 Results Summary
| Model         | Accuracy | Precision (True) | Recall (True) | F1-Score (True) | ROC-AUC |
|---------------|----------|------------------|---------------|-----------------|---------|
| Decision Tree | 0.89     | 0.53             | 0.54          | 0.54            | 0.7410  |
| Random Forest | 0.92     | 0.67             | 0.49          | 0.56            | 0.9474  |
| XGBoost       | 0.92     | 0.69             | 0.56          | 0.62            | 0.9546  |
| AdaBoost      | 0.90     | 0.72             | 0.25          | 0.38            | 0.9366  |

---

## 📌 Insights
- **XGBoost** achieved the highest ROC-AUC score, making it the best at distinguishing between positive and negative cases.
- **Random Forest** had slightly lower recall for the positive class but still performed well.
- **AdaBoost** had high precision but very low recall, indicating it predicts "yes" less often but is usually correct when it does.
- **Decision Tree** is interpretable but underperforms compared to ensemble methods.

---

## 🚀 How to Run
```bash
# Clone repository
git clone https://github.com/your-username/bank-marketing-subscription.git
cd bank-marketing-subscription

# Install dependencies
pip install -r requirements.txt

# Run Jupyter Notebook
jupyter notebook
