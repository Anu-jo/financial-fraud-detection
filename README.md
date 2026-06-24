Project Overview

Financial fraud detection is a critical challenge faced by banks, financial institutions, and online payment systems. Due to the increasing volume of digital transactions, identifying fraudulent activities accurately and efficiently is essential to reduce financial losses and protect customers.

This project applies Big Data Analytics and Machine Learning techniques to detect fraudulent financial transactions using a large-scale credit card transaction dataset. The solution leverages PySpark for distributed data processing and compares the performance of three classification algorithms:

Support Vector Machine (SVM)
Random Forest Classifier
Artificial Neural Network (ANN)

The objective is to evaluate the effectiveness of these algorithms in identifying fraudulent transactions and determine the most suitable model for fraud detection.

🎯 Objectives
Process large-scale financial transaction data using PySpark.
Perform data validation and preprocessing.
Analyze feature relationships through visualization.
Apply feature scaling techniques.
Train and evaluate multiple machine learning models.
Compare model performance using classification metrics.
Identify the best-performing model for fraud detection.
📊 Dataset

The project uses the Credit Card Fraud Detection Dataset, containing anonymized transaction records.

Dataset Information
Attribute	Description
Time	Time elapsed between transactions
V1-V28	PCA-transformed confidential transaction features
Amount	Transaction amount
Class	Target variable (0 = Genuine, 1 = Fraudulent)
Dataset Statistics
Total Transactions: 284,807
Fraudulent Transactions: 492
Genuine Transactions: 284,315
Features: 30 numerical features
Highly imbalanced dataset
🛠️ Technologies Used
Programming Language
Python
Big Data Processing
PySpark
Apache Spark
Machine Learning
Scikit-Learn
TensorFlow / Keras
Data Analysis
Pandas
NumPy
Data Visualization
Matplotlib
Seaborn
Development Environment
Google Colab
Jupyter Notebook
🔄 Project Workflow
1. Data Loading
Create Spark Session
Load dataset using PySpark DataFrames
2. Data Validation
Schema inspection
Data type verification
Missing value detection
Statistical summaries
3. Exploratory Data Analysis
Transaction distribution analysis
Correlation analysis
Fraud vs Genuine transaction analysis
4. Feature Engineering
Added unique transaction identifiers
Prepared features for model training
5. Feature Scaling

Applied MinMaxScaler to normalize transaction features and improve model performance.

6. Model Development

Three machine learning algorithms were implemented and compared:

Support Vector Machine (SVM)

A supervised learning algorithm that identifies an optimal decision boundary between fraudulent and genuine transactions.

Random Forest Classifier

An ensemble learning algorithm that combines multiple decision trees to improve prediction accuracy and reduce overfitting.

Artificial Neural Network (ANN)

A deep learning model capable of learning complex patterns and nonlinear relationships within transaction data.

📈 Data Visualization

The project includes visual analysis using:

Correlation Heatmap
Feature Relationship Analysis
Transaction Distribution Analysis
Sample Visualization

✔ Correlation Heatmap

✔ Feature Correlation Analysis

✔ Fraud Distribution Insights

🏆 Model Performance Comparison

The models were evaluated using:

Accuracy
Precision
Recall
F1-Score
Confusion Matrix
Results
Model	     Accuracy	Precision	Recall	F1-Score
SVM	          0.94	 High	     High	  High
ANN	          0.95	 High      High	  High
Random Forest	1.00	 1.00	     1.00	  1.00
📊 Detailed Findings
Support Vector Machine (SVM)
Accuracy: 94%
Strong classification performance
High precision and recall for both classes
Performed particularly well in detecting fraudulent transactions
Artificial Neural Network (ANN)
Accuracy: 95%
Demonstrated strong learning capability for complex transaction patterns
Achieved balanced performance across both fraud and non-fraud classes
Random Forest Classifier
Accuracy: 100%
Perfect classification performance
Precision: 1.00
Recall: 1.00
F1-Score: 1.00
Correctly classified all fraudulent and non-fraudulent transactions
