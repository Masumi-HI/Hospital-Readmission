# 🏥 Hospital Readmission Risk Analysis

## Project Overview

Hospital readmissions are a critical quality and cost metric in healthcare. This project analyzes patient-level hospital data to identify key factors associated with 30-day readmissions and builds a predictive model to highlight high-risk patients.

The goal is to:

* Understand patterns associated with hospital readmissions
* Identify the most influential risk factors
* Demonstrate the use of machine learning to support clinical and operational decision-making

---

## Dataset

The dataset includes patient demographics, clinical conditions, utilization history, and hospital-related variables.
The target variable indicates whether a patient was readmitted within 30 days of discharge.

---

## Tools & Technologies

* **Python**
* **Pandas / NumPy** – data cleaning and transformation
* **Matplotlib / Seaborn** – exploratory visualizations
* **Scikit-learn** – machine learning and model evaluation
* **Jupyter Notebook**

---

## Project Workflow

### 1. Data Loading & Exploration

* Loaded the hospital readmissions dataset
* Reviewed data types, missing values, and summary statistics
* Identified categorical and numerical variables

### 2. Data Preprocessing

* Encoded the target variable (readmitted vs not readmitted)
* Converted categorical features into numeric form using label encoding
* Ensured data was suitable for machine learning models

### 3. Exploratory Data Analysis (EDA)

* Examined readmission distribution
* Analyzed relationships between readmission and:

  * Length of stay
  * Number of procedures
  * Number of diagnoses
  * Previous inpatient and emergency visits
* Visualized patterns using bar charts and distribution plots

### 4. Feature Engineering

* Selected clinically and operationally relevant variables
* Prepared feature matrix and target vector
* Split data into training and testing sets

### 5. Modeling

* Trained a **Random Forest Classifier**
* Evaluated model performance using:

  * Accuracy
  * Classification report (precision, recall, F1-score)
* Extracted and visualized feature importance scores

### 6. Risk Factor Identification

* Ranked features based on Random Forest importance
* Identified the **top risk factors** contributing to hospital readmission
* Visualized top 5 and top 20 predictors

---

## Key Results

* The model successfully identified patients at higher risk of readmission
* Utilization history and clinical complexity emerged as strong predictors
* Feature importance analysis provided interpretable insights for healthcare stakeholders

---

## Business & Clinical Impact

* Enables early identification of high-risk patients
* Supports targeted interventions such as care coordination and discharge planning
* Can help reduce avoidable readmissions and associated costs
* Demonstrates how analytics can support value-based care initiatives

---

## Future Improvements

* Hyperparameter tuning for improved performance
* Handling class imbalance using resampling techniques
* Incorporating social determinants of health
* Comparing additional models (Logistic Regression, XGBoost)
* Integrating the model into dashboards for operational use

---

## 2️⃣ Observations & Key Findings (Detailed)

You can reference these during interviews or add them as markdown sections in the notebook.

### 🔍 Data Observations

* The dataset contains a mix of demographic, clinical, and utilization-related variables
* Readmission is a **binary classification problem**
* Utilization-related features show strong signals for predicting readmission

### 📊 Exploratory Analysis Observations

* Patients with **higher prior inpatient visits** tend to have higher readmission rates
* Increased **number of diagnoses** is associated with higher readmission risk
* Longer **length of stay** often correlates with patient complexity and readmission
* Emergency and inpatient utilization history are strong indicators of future readmissions

### 🤖 Model Observations

* Random Forest performs well due to its ability to capture non-linear relationships
* Feature importance adds interpretability, which is critical in healthcare analytics
* The model balances predictive power with explainability

### ⭐ Top Risk Factors (High-Level)

Although exact values depend on the dataset, the model consistently prioritizes:

* Prior inpatient visits
* Number of diagnoses
* Length of hospital stay
* Number of procedures
* Emergency department utilization

These align well with real-world clinical intuition.


## 📌 Conclusion

In this analysis, we explored hospital readmission data to identify key drivers of 30-day readmissions and developed a machine learning model to assess patient risk. Through exploratory data analysis, we observed that prior utilization patterns, clinical complexity, and length of stay play a significant role in readmission likelihood.

A Random Forest model was used to capture non-linear relationships between patient characteristics and readmission outcomes. Feature importance analysis revealed that utilization history and diagnosis burden are among the most influential predictors, reinforcing known clinical and operational insights.

This project demonstrates how data science can support healthcare decision-making by:

* Identifying high-risk patients early
* Informing targeted care management strategies
* Supporting value-based care and cost reduction efforts

With further refinement and integration into clinical workflows, this approach can help healthcare organizations reduce avoidable readmissions while improving patient outcomes.

Just tell me 👍
