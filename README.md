# Explainable Customer Churn Prediction and Retention Recommendation System

## 📌 Project Overview

Customer churn is a major challenge for subscription-based businesses. This project develops a Machine Learning system that predicts whether a customer is likely to leave a service and assigns a churn risk level.

The system goes beyond basic churn prediction by using feature engineering, multiple Machine Learning models, cross-validation, threshold analysis, explainability, and retention recommendations.

---

## 🎯 Objectives

- Predict customer churn using Machine Learning.
- Compare multiple classification algorithms.
- Apply data preprocessing and feature engineering.
- Evaluate models using Accuracy, Precision, Recall, F1-Score and ROC-AUC.
- Apply Stratified K-Fold Cross-Validation.
- Identify important factors affecting customer churn.
- Assign customers into Low, Medium and High risk categories.
- Provide suitable customer retention recommendations.

---

## 📊 Dataset

The project uses the **Telco Customer Churn Dataset**.

- Number of customers: 7,043
- Original features: 21
- Target variable: Churn
- Problem type: Binary Classification

The dataset contains information such as:

- Customer tenure
- Monthly charges
- Total charges
- Contract type
- Payment method
- Internet service
- Services subscribed by the customer

---

## ⚙️ Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy
- SHAP
- KaggleHub

---
🧠 Machine Learning Models
The following classification algorithms were implemented:
1. Logistic Regression
2. Decision Tree
3. K-Nearest Neighbors (KNN)
4. Support Vector Machine (SVM)
5. Random Forest

🔧 Feature Engineering
Additional features were created to improve the model:
- Estimated Lifetime Value
- Average Monthly Spend
- Tenure Group
- High Monthly Charge indicator

📈 Model Evaluation
The models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
Stratified 5-Fold Cross-Validation was also used to evaluate model consistency.

🏆 Final Model
The best-performing model selected for the final prediction system was:
Logistic Regression
Final performance on the test dataset:
Metric	Score
Accuracy	80.13%
Precision	65.88%
Recall	52.14%
F1-Score	58.21%
ROC-AUC	84.49%


🎚️ Threshold Optimization
Instead of using only the default 0.50 classification threshold, different thresholds were evaluated.
A threshold of 0.35 was selected because it provided a better balance for the churn-retention objective, particularly improving recall.
At threshold 0.35:
- Accuracy: 77.22%
- Precision: 55.56%
- Recall: 70.86%
- F1-Score: 62.28%
Higher recall is useful in churn prediction because identifying more potentially departing customers allows the company to take preventive retention actions.

🔍 Explainable AI
Feature importance and SHAP-based analysis were used to understand the factors associated with customer churn.
Important features identified include:
- Tenure
- Total Charges
- Estimated Lifetime Value
- Monthly Charges
- Average Monthly Spend
The system therefore provides not only a prediction but also an explanation of the important factors influencing churn.

🚦 Churn Risk Classification
Customers are classified according to predicted churn probability:
Probability	Risk
< 35%	LOW
35% – < 60%	MEDIUM
≥ 60%	HIGH


💡 Retention Recommendations
LOW Risk
Maintain regular customer engagement and provide loyalty benefits.
MEDIUM Risk
Provide personalized loyalty offers and increase customer engagement.
HIGH Risk
Provide personalized retention discounts, long-term contract offers and priority support.

🔮 Future Scope
- Deploy the model as a web application.
- Add real-time customer prediction.
- Improve explainability with individual customer SHAP explanations.
- Add customer segmentation using clustering.
- Integrate the system with CRM platforms.
- Develop automated retention campaigns.
- 
---

## 📊 Results & Visualizations

### Model Comparison

The project compares five classification models based on Accuracy, Precision, Recall, F1-Score and ROC-AUC.

![Model Comparison](screenshots/model_comparison.png)

---

### Confusion Matrix

The confusion matrix shows the classification performance of the final Logistic Regression model.

![Confusion Matrix](screenshots/confusion_matrix.png)

---

### ROC Curve

The Logistic Regression model achieved an ROC-AUC score of approximately **0.845**.

![ROC Curve](screenshots/roc_curve.png)

---

### Feature Importance

The feature importance analysis identifies the major factors associated with customer churn.

![Feature Importance](screenshots/feature_importance.png)

---

### Threshold Analysis

Different classification thresholds were evaluated. A threshold of **0.35** was selected to improve churn detection and achieve a better F1/Recall balance.

![Threshold Analysis](screenshots/threshold_analysis.png)

---

### Customer Churn Prediction

The system generates an individual churn probability, risk level and retention recommendation for a customer.

![Customer Prediction](screenshots/customer_prediction.png)
## 🔄 Project Workflow

```text
Dataset
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Feature Engineering
   ↓
Encoding & Scaling
   ↓
Train-Test Split
   ↓
Multiple ML Models
   ↓
Model Evaluation
   ↓
Cross Validation
   ↓
Best Model Selection
   ↓
Threshold Optimization
   ↓
Churn Prediction
   ↓
Risk Classification
   ↓
Explainability
   ↓
Retention Recommendation



👩‍💻 Author
Riya Sharma
B.Tech Electronics & Communication Engineering
Specialization: Artificial Intelligence & Machine Learning
