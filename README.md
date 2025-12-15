# Predicting Academic Performance Based on Student Behavior

## 📌 Project Overview
This project applies Data Mining techniques to analyze how students' daily habits—such as study time, sleep quality, and social media usage—impact their academic performance. Using the **CRISP-DM** methodology, we aim to predict student exam scores and identify students "at risk" of failure before they take the exam.

## 🎯 Objectives
1.  **Regression Model:** Predict the exact `exam_score` based on lifestyle and study habits.
2.  **Classification Model:** Categorize students as **"At Risk"** (Score < 60) or **"Safe"** to enable early intervention.
3.  **Feature Analysis:** Determine which factors (e.g., Attendance vs. Sleep) have the strongest correlation with success.

## 📂 Dataset
The dataset is sourced from Kaggle: **Student Habits vs Academic Performance**.
- **Rows:** 1,000 Students
- **Columns:** 16 Features (Academic, Lifestyle, Demographic)
- **Target Variable:** `exam_score` (0-100)

## 🛠️ Methodology (KDD Process)
1.  **Preprocessing:** Handling missing values, removing duplicates, and outlier detection.
2.  **Transformation:**
    - **One-Hot Encoding:** For categorical variables like `gender` and `internet_quality`.
    - **Feature Engineering:** Created new metrics:
        - `Study_Intensity`: Combines study hours and session frequency.
        - `Well_Being_Score`: Aggregates sleep and physical activity.
3.  **Modeling:**
    - **Linear Regression & Random Forest:** For score prediction.
    - **Logistic Regression & Decision Tree:** For risk classification.

## 🚀 How to Run
1.  Clone this repository.
2.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3.  Open `analysis_notebook.ipynb` in Jupyter Notebook or Google Colab.
4.  Run all cells to generate the analysis and visualizations.

## 📊 Key Results
- **Top Predictor:** `attendance_percentage` showed the highest correlation with exam scores.
- **Negative Impact:** High `social_media_hours` is strongly correlated with lower grades.
- **Model Accuracy:** The Regression model achieved an RMSE of [Insert Your Result Here] on the test set.

## 👥 Authors
- Sardor Kurbonmurodov
- Yazan Mousa
- İrem Batıgün
- Ece Mina Örenler

**University of Castilla-La Mancha (UCLM)** - Data Mining Course