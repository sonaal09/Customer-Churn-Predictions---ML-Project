README - Customer Churn Prediction Project
------------------------------------------

Student Name: Sonaal Rawat  
Student ID: 23223310  
Course: IS41070 – Machine Learning Foundations (2024/25 Summer)  
Submission Date: 25 July 2025  

Overview:
---------
This project aims to predict customer churn using five different machine learning models:

1. Logistic Regression  
2. Decision Tree  
3. Random Forest  
4. XGBoost  
5. Support Vector Machine (SVM)

Each model was developed in a separate notebook for better modularity, tuning, and analysis. SMOTE was applied selectively to address class imbalance. All models were tuned using either GridSearchCV or RandomizedSearchCV. Final evaluations were conducted on a holdout test set.

Folder Structure:
-----------------

23223310_ML_PROJECT/
├── Data Report.docx                 # Final written report
├── README.txt                       # Project documentation
├── requirements.txt                 # Python package dependencies
│
├── htmls/                           # Exported HTML versions of notebooks
│   ├── EDA.html
│   ├── Logistic_Regression.html
│   ├── Decision_Tree.html
│   ├── Random_Forest.html
│   ├── XGBoost.html
│   └── SVM.html
│
└── notebook_and_ml/                # Jupyter notebooks + datasets
    ├── EDA.ipynb
    ├── Model_1_Logistic_Regression.ipynb
    ├── Model_2_Decision_Tree.ipynb
    ├── Model_3_Random_Forest.ipynb
    ├── Model_4_XGBoost.ipynb
    ├── Model_5_SVM.ipynb
    ├── train.csv
    ├── val.csv
    ├── test.csv
    ├── cleaned_data.csv
    └── raw_data.csv

Instructions:
-------------
- All notebooks are self-contained and can be run independently using Jupyter Notebook.
- Data files should remain in notebook_and_ml/ to ensure paths are correct.
- Use `requirements.txt` to install necessary dependencies.
- View HTML files in the `htmls/` folder for quick reference.
- Main findings, charts, and business recommendations are detailed in `Data Report.docx`.

Contact: sonaal.rawat@ucdconnect.ie