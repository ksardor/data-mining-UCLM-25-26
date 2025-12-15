# Predicting academic performance based on student behavior

## 📌 Project overview
This project applies Data Mining techniques to analyze how students' daily habits—such as study time, sleep quality, and social media usage—impact their academic performance. Using the **CRISP-DM** methodology, we aim to predict student exam scores and identify students "at risk" of failure before they take the exam.

## 🎯 Objectives
1.  **Regression model:** Predict the exact `exam_score` based on lifestyle and study habits.
2.  **Classification model:** Categorize students as **"At Risk"** or **"Safe"** to enable early intervention.
3.  **Feature analysis:** Determine which factors have the strongest correlation with success.

## 📂 Dataset
The dataset is sourced from Kaggle: **Student Habits vs Academic Performance**.
- **Rows:** 1,000 students
- **Columns:** 16 features (academic, lifestyle, demographic)
- **Target variable:** `exam_score` (0-100)

## 🛠️ Methodology (KDD process)
1.  **Preprocessing:** Handling missing values, removing duplicates, and outlier detection.
2.  **Transformation:**
    - **One-hot encoding:** For categorical variables like `gender` and `internet_quality`.
    - **Feature engineering:** Created new metrics:
        - `Study_Intensity`: Combines study hours and session frequency.
        - `Well_Being_Score`: Aggregates sleep and physical activity.
3.  **Modeling:**
    - **Linear regression & Random Forest:** For score prediction.
    - **Logistic regression & Decision Tree:** For risk classification.

## 📊 Key Results
- **Top predictor:** `attendance_percentage` showed the highest correlation with exam scores.
- **Negative impact:** High `social_media_hours` is strongly correlated with lower grades.
- **Model Accuracy:** The Regression model achieved an RMSE of **94.50%** on the test set.

## 👥 Authors
- Sardor Kurbonmurodov
- Yazan Mousa

**University of Castilla-La Mancha** - Data Mining Course
