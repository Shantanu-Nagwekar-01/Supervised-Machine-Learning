# ❤️ Framingham Heart Disease Prediction

This project uses **Logistic Regression** to predict whether a person has a 10-year risk of coronary heart disease (CHD), based on health and lifestyle attributes from the Framingham dataset.

---

## 🗂 Dataset Overview

- **Source**: Framingham Heart Study
- **Records**: 4,238
- **Features**: 15 (age, BMI, BP, glucose, etc.)
- **Target**: `TenYearCHD` (1 = likely CHD in 10 years, 0 = no risk)

---

## 🔧 Process Overview

1. Data Cleaning & Imputation
2. Feature Scaling with `StandardScaler`
3. Model Training using `LogisticRegression`
4. Evaluation:
   - Accuracy
   - Precision, Recall, F1-score
   - Confusion Matrix
   - ROC Curve & AUC

---

## ⚙️ Tools Used

- Python 3
- pandas, NumPy
- scikit-learn
- matplotlib

---

## 📊 Model Performance

| Metric       | Training Set | Test Set |
|--------------|--------------|----------|
| Accuracy     | ~68%         | ~67%     |
| Recall (1)   | ~70%         | ~58%     |
| Precision (1)| ~28%         | ~25%     |
| ROC AUC      | ~0.72        | ~0.71    |

> Focus was on improving recall for the positive class (CHD risk), since false negatives are more dangerous in healthcare.

---

## 📈 Visualizations

- Heatmap of feature correlations
- Confusion matrix
- ROC curve

---

## ✅ Insights

- Feature scaling significantly improved recall
- Precision-recall tradeoff observed with logistic regression
- ROC AUC suggests the model performs better than random guessing

---

## 🚀 Future Work

- Use SMOTE for class balancing
- Try advanced models: Random Forest, XGBoost
- Build a custom logistic regression using NumPy
- Deploy via Flask/FastAPI for real-world use

---

## ✍️ Author

**Shantanu Nagwekar**

> Explore, fork, or improve! Feedback is welcome.
