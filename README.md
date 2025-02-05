# Prediabetes Risk Assessment

This project aims to assess the risk of prediabetes among Indian youngsters aged from 15-25 based on various health and lifestyle factors.I aim to identify key factors that contribute to the risk of prediabetes and develop predictive models to assess individual risk levels. This can help in early detection and preventive measures to reduce the incidence of diabetes.

## Table of Contents

1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Project Structure](#project-structure)
4. [Key Features and Methods](#key-features-and-methods)
5. [Usage](#usage)
6. [Technologies Used](#technologies-used)
7. [Results](#results)
8. [Future Improvements](#future-improvements)

## Overview

Prediabetes is a condition that often precedes type 2 diabetes, characterized by blood sugar levels that are higher than normal but not high enough to be classified as diabetes. This project focuses on analyzing various factors such as lifestyle habits, genetic predisposition, and health metrics to predict prediabetes risk among young adults (ages 15-25) in India.

## Dataset

The dataset, "Diabetes in Young Adults in India," was sourced from Kaggle. It contains 100,000 records of synthetic data designed to capture:

- Demographic details
- Genetic risk factors
- Lifestyle habits
- Health metrics
- Diabetes outcomes

### Key Columns:

- **ID:** Unique identifier for each individual
- **Age, Gender, Region:** Demographic details
- **Family_Income:** Household income
- **Family_History_Diabetes:** Family history of diabetes
- **Parent_Diabetes_Type:** Type of diabetes in parents
- **Genetic_Risk_Score:** Genetic predisposition score
- **BMI, Physical_Activity_Level:** Health and lifestyle metrics
- **Fast_Food_Intake, Smoking, Alcohol_Consumption:** Lifestyle habits
- **Fasting_Blood_Sugar, HbA1c, Cholesterol_Level:** Key health indicators
- **Prediabetes:** Target variable indicating prediabetes status

## Project Structure

```
Prediabetes_Risk_Assessment/
│
├── data/               # Data Files
│   ├── raw_data.csv    # Original dataset
│   ├── processed_data.csv  # Preprocessed dataset
│   ├── feature_engineered_data .csv  # Feature engineered dataset
│    
├── notebooks/          # Jupyter notebooks 
    ├── 1_data_processing.ipynb
    ├── 2_eda.ipynb
    ├── 3_feature_engineering.ipynb
    ├── 4_model_building.ipynb


```

## Key Features and Methods

1. **Data Processing:**
   - Handled null values and inconsistencies in the dataset.
   - Encoded categorical variables and normalized numerical data.

2. **Exploratory Data Analysis (EDA):**
   - Investigated distributions, correlations, and key patterns in the data.
   - Identified key factors influencing prediabetes risk.

3. **Feature Engineering:**
   - Created new features such as BMI-Activity Risk categories and Stress-Sleep Ratio.
   - Selected features based on importance scores.
   - Performed advanced EDA on the feature engineered data to identify patterns and insights.

4. **Model Training:**
   - Trained machine learning models (e.g., logistic regression, random forest).
   - Evaluated performance using accuracy, precision, recall, and F1-score.


## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/Santheeppa/Prediabetes_Risk_Assessment.git
   cd Prediabetes_Risk_Assessment
   ```
2. Run Jupyter notebooks for data processing, analysis, and training:
   ```bash
   jupyter notebook
   ```

## Technologies Used

- **Python Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn
- **Jupyter Notebook:** For interactive data exploration and analysis

## Results

Our diabetes prediction models achieved ~70% accuracy across all approaches ( Logistic Regression: 69.82%, XGBoost: 69.28%, Random Forest: 69.75% ,KNeighborsClassifier: 62.75%). Logistic Regression emerged as the best performer with more balanced predictions. Key predictors include BMI, HbA1c, Sleep Hours, Fast Food Intake, Physical Activity, Blood Sugar levels, Cholesterol, Family History Diabetes, Parent Diabetes Type, and Genetic Risk Score.

---

Hey there! 😊

I just wanted to share a little disclaimer about this project. I know it might not be perfect, but I'm committed to learning from my mistakes and improving along the way. Your feedback is incredibly valuable to me, so if you notice anything that could be better or needs correcting, please feel free to let me know. I'm always eager to learn and grow!
Thanks so much for your support and understanding!

Cheers, [Santheeppa]
---
Feel free to contribute by submitting issues or pull requests.

