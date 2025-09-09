
 

# Task 2: End-to-End ML Pipeline with Scikit-learn Pipeline API

## 📌 Objective
The goal of this task is to build a **reusable and production-ready machine learning pipeline** for predicting **customer churn** using the **Telco Churn Dataset**.  
The pipeline should integrate **data preprocessing**, **model training**, **hyperparameter tuning**, and **model export**, ensuring that it can be deployed seamlessly in real-world applications.

---

## 🔧 Methodology / Approach
1. **Data Preprocessing with Pipeline**
   - Handle missing values and categorical encoding.
   - Apply **OneHotEncoder** for categorical features.
   - Apply **StandardScaler** for numerical features.
   - Combine transformations using **ColumnTransformer** inside a `Pipeline`.

2. **Model Training**
   - Train **Logistic Regression** and **Random Forest** classifiers.
   - Encapsulate preprocessing + model training into a **single pipeline** for consistency.

3. **Hyperparameter Tuning**
   - Use **GridSearchCV** for systematic hyperparameter optimization.
   - Evaluate model performance with cross-validation.

4. **Model Export**
   - Save the best performing pipeline using **joblib**.
   - Ensure the pipeline includes preprocessing steps, making it ready for production use without manual feature engineering.

---

## 📊 Key Results / Observations
- **Pipeline Efficiency**: Encapsulating preprocessing + training ensured consistent handling of data during both training and inference.
- **Best Model**: Random Forest achieved higher predictive performance compared to Logistic Regression on churn prediction.
- **Hyperparameter Tuning**: GridSearchCV improved model accuracy and reduced overfitting by finding optimal parameters.
- **Reusability**: Exported pipeline (`.joblib`) can be directly loaded and used for predictions on new data without retraining or reapplying preprocessing steps.
- **Production Readiness**: The end-to-end pipeline design ensures scalability and deployment feasibility in real-world scenarios.

---

## 🚀 Skills Gained
- Building **end-to-end ML pipelines** with Scikit-learn.
- Applying **data preprocessing** systematically using `Pipeline` and `ColumnTransformer`.
- Performing **hyperparameter tuning** with `GridSearchCV`.
- Exporting and reusing ML models with **joblib**.
- Following **production-readiness practices** for machine learning workflows.
