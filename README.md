# Customer Churn Prediction – Telecom Sector
Project Overview

This project focuses on predicting customer churn in the telecommunications sector using machine learning. Churn occurs when a customer discontinues their service, which can be very costly for telecom providers. Since retaining existing customers is generally cheaper than acquiring new ones, an effective churn prediction model can provide significant business value.

The main objective was to build models that identify customers at risk of leaving, enabling proactive retention strategies.

# Business Problem

The dataset used was imbalanced: around 27% of customers had churned, while 73% had not. Because of this, the project prioritized recall (sensitivity) for churners. Correctly identifying churners was more important than overall accuracy, since missing a churner can mean losing a customer and revenue.

# Methodology

I built and compared five machine learning models:

Logistic Regression

Decision Tree

Random Forest

XGBoost

Support Vector Machine (SVM)

Each model was developed in a separate notebook for clarity and deeper testing. Techniques like SMOTE oversampling, scaling, and hyperparameter tuning (GridSearchCV/RandomizedSearchCV) were applied where appropriate.

The dataset was split into training (70%), validation (15%), and test (15%) using stratified sampling to preserve class balance.

# Evaluation Metrics

To evaluate the models, I used:

Recall (for churners)

ROC AUC

F1-Score

Confusion Matrix

# Results

Decision Tree showed the biggest improvement after tuning, reaching ROC AUC of 0.91.

Random Forest and XGBoost both performed very well, each surpassing ROC AUC of 0.90.

SVM improved moderately, while Logistic Regression remained stable but interpretable.

Best Model: XGBoost

Achieved 83% recall for churners on the test set.

Prioritized identifying churners at the expense of some false positives.

Selected as the most suitable model given the business requirement to minimize lost customers.

# Business Impact

The chosen model can:

Flag customers likely to churn so companies can offer loyalty programs, discounts, or personalized outreach.

Integrate into CRM systems for proactive retention strategies.

Help reduce revenue loss from customer turnover.

Limitations and Future Work

The dataset was relatively small (~7,000 rows). Larger or real-time datasets could improve generalization.

Future improvements could include:

More feature engineering (e.g., complaint history, usage patterns)

Explainability methods (e.g., SHAP values)

Ensemble approaches or time-aware validation

# Conclusion

This project demonstrated how machine learning can be applied to predict telecom customer churn. After comparing five models, XGBoost was selected as the most effective, achieving high recall and strong business relevance.

References

Scikit-learn Documentation

XGBoost Documentation

Google Colab Notebook (Project Work)
