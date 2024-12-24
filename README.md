Credit Card Fraud Detection System
Overview
This project focuses on building a robust credit card fraud detection system using various machine learning techniques. The goal is to accurately identify fraudulent transactions and minimize false positives to ensure a secure and trustworthy environment for financial transactions.

Dataset
Source: creditcard.csv

Description: The dataset contains credit card transactions, including both legitimate and fraudulent ones. It includes features such as time, transaction amount, and 28 principal components obtained using PCA.

Key Features
Time: Time elapsed between this transaction and the first transaction in the dataset.

V1 to V28: Principal components obtained with PCA.

Amount: Transaction amount.

Class: Target variable (0: Non-Fraud, 1: Fraud).

Steps Involved
1. Data Preprocessing
Data Inspection: Loading the dataset, displaying the first few rows, and visualizing the class distribution.

Handling Missing Values: Removing rows with missing values in the 'Class' column.

Feature and Target Separation: Separating features (X) and target variable (y).

Balancing the Dataset: Using SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset.

2. Feature Scaling
Applying StandardScaler to standardize the features, ensuring all features contribute equally to the model's learning process.

3. Data Splitting
Splitting the dataset into training and testing sets to evaluate model performance on unseen data.

4. Feature Selection and Importance
Correlation Analysis: Identifying the most relevant features.

Recursive Feature Elimination (RFE): Selecting important features.

Random Forest Feature Importance: Evaluating feature importance using a Random Forest model.

5. Model Training and Evaluation
Training and evaluating multiple models including Logistic Regression, Decision Tree, Random Forest, XGBoost, and SVM.

Assessing models using metrics such as accuracy, precision, recall, F1-score, and ROC-AUC.

Summarizing and comparing the evaluation metrics of all models.

6. Hyperparameter Tuning
Optimizing model performance using:

Grid Search: Exhaustive search through a specified parameter grid.

Random Search: Sampling random combinations of parameters.

Bayesian Optimization: Using a probabilistic model to find the best parameters efficiently.

Model Performance
Evaluation Metrics
Model	Accuracy	Precision	Recall	F1-Score	ROC-AUC
Logistic Regression	0.9916	0.9934	0.9897	0.9915	0.9994
Decision Tree	0.9996	0.9994	0.9997	0.9996	0.9996
Random Forest	0.9999	1.0000	0.9999	0.9999	1.0000
XGBoost	0.9997	0.9999	0.9996	0.9997	1.0000
SVM	0.9992	0.9985	1.0000	0.9992	1.0000
Model Comparison: ROC-AUC Scores
Include diagram here

Conclusion
This project successfully developed a reliable credit card fraud detection system by:

Performing effective data preprocessing and balancing the dataset.

Selecting relevant features to improve model performance.

Training and evaluating multiple models to find the best-performing one.

Optimizing model performance through hyperparameter tuning.

By following this systematic approach, we achieved high accuracy and ROC-AUC scores, making our fraud detection system robust and effective in identifying fraudulent transactions.

Future Work
Model Deployment: Deploy the model in a production environment for real-time fraud detection.

Continuous Monitoring: Continuously monitor and update the model to adapt to new fraud patterns.

Feature Engineering: Explore additional features that could improve model performance.

References
SMOTE - Synthetic Minority Over-sampling Technique

Random Forest - Scikit-learn

XGBoost - Scikit-learn API
