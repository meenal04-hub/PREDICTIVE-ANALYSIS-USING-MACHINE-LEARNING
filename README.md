# PREDICTIVE-ANALYSIS-USING-MACHINE-LEARNING

**TOPIC** : Credit_Card_Fraud_Detection

**COMPANY** : CODTECH IT Solutions

**NAME** : Meenal Gaikwad

**INTERN ID** : CT6WLXP

**DOMAIN** : Data Analytics

**DURATION** : 6 weeks

**MENTOR NAME** : Neela Santhosh Kumar

**DESCRIPTION** : 

# Credit Card Fraud Detection

**1. Introduction**

Credit card fraud is a major concern in the financial industry, leading to billions of dollars in losses annually. This project focuses on developing a machine learning model to detect fraudulent transactions, helping financial institutions identify suspicious activities in real-time while reducing false positives.

The dataset used in this project contains anonymized transaction data, including transaction amounts, timestamps, and engineered numerical features. Since fraudulent transactions are extremely rare, this presents a highly imbalanced classification problem, requiring advanced data science techniques for effective fraud detection.

**2. Dataset Overview**

The dataset used for this project is the Kaggle Credit Card Fraud Detection Dataset, which contains:

* 284,807 transactions, where only 0.17% are fraudulent.
* 30 features, including:
  * V1-V28 → Anonymized numerical features derived from PCA.
  * Amount → Transaction amount.
  * Time → Time elapsed since the first transaction in the dataset.
    
Due to data imbalance, special techniques are required to enhance fraud detection accuracy.

**3. Data Preprocessing**

To ensure optimal model performance, the following preprocessing steps were performed:

Data Balancing

* SMOTE (Synthetic Minority Oversampling Technique) was used to create synthetic fraudulent transactions.
* Undersampling was applied to reduce the dominance of non-fraudulent transactions.
  
Feature Scaling
* StandardScaler was used to normalize numerical features like Amount and Time to improve model performance.
  
Train-Test Split
* The dataset was divided into 80% training and 20% testing for model evaluation.
  
**4. Model Selection & Training**

Several supervised learning algorithms were tested to classify transactions as fraudulent or legitimate:

**Models Evaluated**

✔ Logistic Regression → A simple baseline model for binary classification.

✔ Random Forest Classifier → An ensemble method known for handling imbalanced data effectively.

✔ XGBoost → A high-performance gradient-boosting algorithm.

✔ Neural Networks → Deep learning applied for advanced feature extraction and fraud detection.

Each model was trained and fine-tuned using hyperparameter optimization techniques to achieve the best performance.

**5. Evaluation Metrics**

Since the dataset is highly imbalanced, accuracy alone is not a reliable metric. Instead, we used:

* Precision & Recall → To measure how well the model identifies fraudulent transactions.
* F1 Score → A balance between precision and recall.
* ROC-AUC Score → To evaluate the trade-off between true positive rate (TPR) and false positive rate (FPR).
  
**Best Model Performance**

✔ Precision: 0.9956

✔ Recall: 0.7184

✔ F1 Score: 0.5565

The selected model effectively detects fraudulent transactions while minimizing false positives.

**6. Deployment**

To make the fraud detection system usable in real-world applications, the final model is integrated into a simple pipeline for real-time fraud detection.

Future Deployment Steps
* Deploying API using Flask/FastAPI for real-time transaction analysis.
* Integrating with a database to handle live transaction data.
* Enhancing the model with deep learning and real-time learning techniques.

**7. Technologies & Tools Used**

* Python
* Pandas & NumPy → Data manipulation & preprocessing
* Scikit-Learn & XGBoost → Machine learning models
* SMOTE (imbalanced-learn) → Data balancing
* Matplotlib & Seaborn → Data visualization
* Flask/FastAPI (for deployment)

**8. Conclusion**

This project successfully demonstrates the use of machine learning for fraud detection. By leveraging data balancing, feature engineering, and advanced classification models, we created a system that can effectively identify fraudulent credit card transactions.

Future enhancements may include deep learning models, real-time learning, and cloud deployment for better scalability and performance.
