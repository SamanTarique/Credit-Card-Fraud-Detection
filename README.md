#  Credit Card Fraud Detection using Machine Learning

##  Project Overview
This project is a **Machine Learning-based Fraud Detection System** that classifies credit card transactions as:

-  Normal (0)
-  Fraud (1)

Using multiple classification algorithms, the best model is selected based on performance metrics.

---
##  Dataset
The dataset is too large to be uploaded on GitHub due to size limitations.

-> [Download Dataset](https://drive.google.com/file/d/1tXxuArcMPaqKBH6QfiwhF32wOy39pEFs/view?usp=sharing)

---

##  ML Pipeline (Step-by-Step)

### 1️) Problem Definition
Fraud detection is a **binary classification problem** in an imbalanced dataset.

---

### 2️) Data Collection
- Credit card transaction dataset
- Features: V1–V28, Time, Amount
- Target: Class (0 = Normal, 1 = Fraud)

---

### 3️) Data Cleaning & Preprocessing
- Removed duplicates
- Handled missing values
- Feature scaling using StandardScaler / RobustScaler

---

### 4️) Exploratory Data Analysis (EDA)
- Class imbalance analysis
- Fraud vs Normal visualization
- Time & Amount distribution study

---

### 5️) Feature Engineering
- Hour extracted from Time
- Created Is_Night feature
- Log transformation on Amount
- Scaled numerical values

---

### 6️) Feature Selection
- Important engineered features selected
- PCA features (V1–V28) handled carefully

---

### 7️) Model Selection
Models used:
- Logistic Regression
- Random Forest
- XGBoost

---

### 8️) Model Training
- Train-test split applied
- SMOTE used for imbalance handling
- Supervised learning approach

---

### 9️) Model Evaluation & Tuning
Metrics used:
- Accuracy
- Precision
- Recall (most important for fraud)
- F1-score
- Confusion Matrix

Hyperparameter tuning done using **GridSearchCV**

---

### 10) Model Deployment & Monitoring
- Best model saved using Joblib
- Continuous monitoring required for fraud pattern changes
- Model retraining when needed

---

##  Best Model Performance

###  Random Forest (Tuned Model)
-  Accuracy: **0.99**
-  Recall (Fraud): **0.99**
-  Lowest Errors: **1257**

 Selected as final production model

---

##  Tech Stack
- Python 
- Pandas & NumPy
- Scikit-learn
- XGBoost
- SMOTE
- Matplotlib & Seaborn
- Joblib

---

##  Future Improvements
- Real-time fraud detection API
- Deep learning models
- Flask / FastAPI deployment
- Continuous learning system

---

##  Author: Saman Tarique
Credit Card Fraud Detection Project using Machine Learning
