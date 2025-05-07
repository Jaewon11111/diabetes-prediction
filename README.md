# 🩺 Diabetes Prediction with Clinical Insights and Machine Learning

This project builds machine learning models (Logistic Regression and Random Forest) to predict diabetes, compares performance metrics, and analyzes model behavior using feature importance and clinical understanding.

> 📄 **[Final Report PDF](./Diabetes_Prediction_Report.pdf)**  
> 💻 **[Jupyter Notebook (Analysis Code)](./Diabetes_Prediction.ipynb)**

---

## 📌 Project Overview

- **Dataset**: [Kaggle - Diabetes Data Set](https://www.kaggle.com/datasets/mathchi/diabetes-data-set)
- **Goals**:  
  - Analyze associations between independent variables and diabetes onset  
  - Clean and preprocess data using medical domain knowledge  
  - Compare model performance using Logistic Regression and Random Forest  
  - Interpret performance differences via feature importance analysis

---

## 🔍 Key Analysis Steps

1. **Definition of Medical Features and Preprocessing Criteria**

2. **Data Preprocessing**  
   - Handle outliers through removal or replacement with mean/median values  
   - Apply log transformation and standard scaling (StandardScaler)  
   - Check multicollinearity using VIF (Variance Inflation Factor)

3. **Model Training and Comparison**  
   - Train `Logistic Regression` and `Random Forest` classifiers  
   - Evaluate using Confusion Matrix, F1 Score, ROC-AUC, etc.

4. **Conclusion**

  - Both models perform well in terms of ROC-AUC  
  - Logistic Regression outperforms in Accuracy, Precision, F1 Score, and ROC-AUC, while Random Forest shows higher Recall  
  - The limited role of the Pregnancies variable in Random Forest may help explain its relatively higher recall

---

## 🧠 Performance Summary

| Model                | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---------------------|----------|-----------|--------|----------|---------|
| Logistic Regression | 0.819    | 0.698     | 0.682  | 0.690    | 0.873   |
| Random Forest       | 0.805    | 0.660     | 0.705  | 0.681    | 0.861   |

- Summary:
  - Logistic Regression: Higher in Accuracy, Precision, F1 Score, ROC-AUC
  - Random Forest: Higher in Recall

---

## 🛠 Tools Used

- Python (Pandas, NumPy, Seaborn, Scikit-learn)
- Jupyter Notebook
- Data preprocessing with clinical context
- PDF report with supporting medical references

---

## 👩‍⚕️ Author

- Name: [Your Name]  
- Education: [Medical School or Major]  
- Interests: Healthcare, Medical AI, Data-driven clinical decision-making, MSL/MA roles  
- Contact: [email or LinkedIn link]

---

## 📎 References

- [Asan Medical Center - Health Information (Korean)](https://www.amc.seoul.kr/)
- [Korean Diabetes Association](https://www.diabetes.or.kr/)
- [Korea Disease Control and Prevention Agency (KDCA) Health Info, etc.](https://health.kdca.go.kr/)
