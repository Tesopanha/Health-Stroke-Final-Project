# Stroke Prediction and Analysis Project

## Project Overview
This project analyzes patient health records to uncover patterns and risk factors linked to stroke. By applying both unsupervised and supervised machine learning techniques, the goal is to classify patients into distinct groups based on their health profiles and risk levels. The insights aim to help healthcare providers implement targeted interventions for those at higher risk, enhancing stroke prevention and management. Predictive models are developed to accurately identify at-risk individuals, enabling earlier intervention and more efficient resource allocation.

## Dataset
- **Source:** [Kaggle - Stroke Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset?resource=download)
- **Description:** The dataset contains patient health records with features such as age, gender, hypertension, heart disease, marital status, work type, residence type, average glucose level, BMI, smoking status, and stroke occurrence.

## Technologies and Tools Used
- **Programming Language:** Python 3
- **Libraries:**
  - pandas, numpy (data manipulation)
  - seaborn, matplotlib (visualization)
  - scikit-learn (preprocessing, modeling, evaluation)
- **Jupyter Notebook** for interactive analysis

## Data Preprocessing
- Checked and handled missing values (e.g., BMI)
- Encoded categorical variables
- Normalized numerical features
- Split data into training and testing sets

## Models and Evaluation
The following machine learning models were trained and evaluated:
- **RandomForestClassifier**
- **LogisticRegression**
- **DecisionTreeClassifier**
- **KNeighborsClassifier**

### Results Summary
- All models achieved high accuracy for classifying non-stroke cases (class 0), but their performance on stroke cases (class 1) was poor due to dataset imbalance.
- The models showed bias towards the majority class (non-stroke), resulting in low precision and recall for the minority class (stroke).
- **Best accuracy:**
  - RandomForestClassifier: ~0.956
  - KNeighborsClassifier: ~0.957
  - DecisionTreeClassifier: ~0.956
  - LogisticRegression: ~0.638
- **Best runtime:** DecisionTreeClassifier and KNeighborsClassifier

## Key Findings
- About 96% of samples did not have a stroke; only 4% had a stroke.
- Most stroke cases were in patients aged 40–85, BMI 20–40, and glucose level 50–130.
- The dataset is highly imbalanced, which affects model performance for minority class prediction.

## Recommendations
- Address class imbalance (e.g., with resampling or advanced algorithms) for better stroke prediction.
- Use the developed models as a baseline for further improvement and real-world deployment.

---

**Author:** [Your Name]
**Date:** July 2025
