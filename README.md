🩺 Insurance Cost Prediction - EDA Project

## 📌 Project Overview

This project aims to perform **Exploratory Data Analysis (EDA)** on an insurance dataset to uncover insights that influence medical insurance charges. The analysis is designed to help **ABC Insurance** make informed decisions regarding premium structures based on various factors such as age, gender, BMI, number of children, smoking habits, and region.

---

## 🧠 Problem Statement

ABC Insurance wants to understand how different features affect healthcare insurance costs. Specifically, the goal is to:

- Identify patterns and trends in insurance charges
- Understand the impact of lifestyle choices (e.g., smoking) on premiums
- Build the foundation for a predictive model to estimate future insurance charges

---

## 🎯 Objective

To analyze the dataset and derive insights that contribute to building a model to **predict medical insurance costs** based on customer attributes.

---

## 🩻 Dataset Information

- **Source**: `insurance.csv`
- **Domain**: Healthcare

| Feature     | Description                                                |
|-------------|------------------------------------------------------------|
| `age`       | Age of the policyholder                                    |
| `sex`       | Gender (`male`, `female`)                                  |
| `bmi`       | Body Mass Index                                            |
| `children`  | Number of children covered under the insurance             |
| `smoker`    | Smoking status (`yes`, `no`)                               |
| `region`    | Residential area (`northeast`, `northwest`, etc.)          |
| `charges`   | Insurance premium charged                                  |

---

## 🛠️ Tools and Libraries Used

- `Python`
- `Pandas` - data manipulation
- `NumPy` - numerical operations
- `Matplotlib`, `Seaborn` - data visualization

---

## 🧪 Steps Performed

1. **Data Import and Setup**
   ```python
   import pandas as pd
   import numpy as np
   import matplotlib.pyplot as plt
   import seaborn as sns
   data = pd.read_csv('insurance.csv')
   ```

2. **Data Inspection**
   - Checked data shape and column types
   - Verified no missing values

3. **Data Exploration**
   - Count plots for categorical features: `region`, `sex`, `smoker`
   - Scatter plots for numerical features vs `charges`: `age`, `bmi`, `children`

4. **Feature vs Feature Visualization**
   - Boxplots, bar plots, and count plots across features
   - Distribution of charges across various regions, BMI ranges, etc.

5. **Insight on Smoking & Charges**
   - Bar plots to visualize correlation between **age vs charges**, and **smoking status vs charges**
   - Noted strong relationship between **smoking status** and **high premiums**

---

## 📈 Key Insights

- **Smokers pay significantly higher premiums** than non-smokers.
- **Age and BMI are positively correlated** with insurance charges.
- Charges **vary across regions**, with the southeast having notably higher average costs.
- Males and females have similar average charges, but distributions vary.

---

## 📊 Sample Visualizations

- `sns.barplot(x='smoker', y='charges')`
- `sns.scatterplot(x='bmi', y='charges')`
- `sns.boxplot(x='children', y='charges')`

*(Note: Visual outputs not included here but were plotted in the analysis.)*

---

## ✅ Future Scope

- Build and evaluate machine learning models to predict `charges`.
- Apply feature scaling and encode categorical variables.
- Use regression techniques for price prediction.
