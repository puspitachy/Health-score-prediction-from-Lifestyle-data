# 🧠 A Machine Learning Approach for Predicting Health Scores from Lifestyle Data

## 📋 Overview
This project applies **machine learning techniques** to predict a person's **Health Score** based on their **lifestyle factors** such as diet quality, exercise frequency, sleep duration, smoking habits, alcohol consumption, BMI, and age.  
By analyzing these variables, the goal is to understand how lifestyle choices impact overall health and to build a predictive model that can guide individuals toward better health outcomes.

---

## 🎯 Objectives
- To clean, preprocess, and analyze lifestyle and health data.
- To visualize relationships between key health indicators.
- To build predictive models that estimate health scores from given features.
- To evaluate model performance using metrics such as **Mean Squared Error (MSE)** and **R² Score**.
- To identify which lifestyle factors most strongly influence overall health.

---

## 📊 Dataset Description
The dataset includes key features such as:

| Feature | Description | Type |
|----------|--------------|------|
| Age | Age of the individual | Numeric |
| BMI | Body Mass Index | Numeric |
| Exercise_Frequency | How often the person exercises per week | Numeric |
| Diet_Quality | Self-rated diet quality score | Numeric |
| Sleep_Hours | Average hours of sleep per night | Numeric |
| Alcohol_Consumption | Units of alcohol consumed per week | Numeric |
| Smoking_Status | Whether the person smokes (0 = No, 1 = Yes) | Categorical |
| Health_Score | Overall health rating (Target variable) | Numeric |

---

## ⚙️ Project Workflow

### 1. **Data Preprocessing**
- Handled missing values and ensured clean data.
- Separated features into numeric and categorical types.
- Scaled numeric data using `StandardScaler`.
- Encoded categorical features using `OneHotEncoder`.

### 2. **Splitting the Dataset**
- The dataset was split using `train_test_split`:
  - 70% for training
  - 30% for testing  
  ```python
  x_train, x_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)
