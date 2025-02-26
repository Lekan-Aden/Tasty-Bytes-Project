# Tasty Bytes – Predicting Popular Recipes

## Overview  
This project was completed as part of my **Data Scientist certification on DataCamp**.  

*Tasty Bytes* started as a recipe search engine during the COVID-19 pandemic and has since evolved into a subscription-based meal planning service. To increase engagement and subscriptions, the company aims to optimize the selection of homepage recipes.  

## Problem Statement  
Currently, recipe selection for the homepage is based on personal preference, leading to inconsistent traffic results. Since popular recipes can boost traffic by up to **40%**, a data-driven approach is needed to systematically predict high-performing recipes and improve engagement.  

## Objective  
The objective here is to develop a predictive model to identify popular recipes with at least **80% accuracy**, ensuring that the homepage features high-performing recipes to drive traffic and subscriptions.  

## Key Steps & Methodology  
1. **Data Cleaning & Validation**  
   - Handled missing values and formatting inconsistencies.

2. **Exploratory Data Analysis (EDA) & Feature Engineering**  
   - Identified key predictors of recipe popularity.  
   - Created new features to enhance model performance.  

3. **Model Development & Evaluation**  
   - Trained and evaluated **Logistic Regression** and **Random Forest** models.  
   - Performed hyperparameter tuning to optimize accuracy.  
   - Evaluated models using **accuracy** and **F1-score**. 

## Findings, Model Choice, Recommendations  
- **Recipe category** was the strongest single predictor of popularity, achieving **77.89% accuracy** in both Logistic Regression and Random Forest models.  
- However, I ultimately selected a **Logistic Regression model trained on multiple features (76.84% accuracy)** because relying on a single feature is unrealistic in real-world applications. While the single-feature model had slightly higher accuracy, a multi-feature approach provides a more robust and generalizable model.  
- High-traffic categories: **Vegetables, Pork, Potatoes, Meat** → should be prioritized on the homepage.  
- Low-traffic categories: **Beverages, Chicken, Breakfast** → should be deprioritized or analyzed further.
- Future improvements: Collect more data and features such as **user ratings, preparation time, and cost** to refine predictions.  

## Tools & Libraries  
- **Python:** Pandas, NumPy, SciPy, Matplotlib, Seaborn, Scikit-learn  
- **Jupyter Notebook**  

## How to Use 
1. Clone the repository:  
   ```bash
   git clone https://github.com/Lekan-Aden/tasty-bytes.git
   cd tasty-bytes
   ```
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
