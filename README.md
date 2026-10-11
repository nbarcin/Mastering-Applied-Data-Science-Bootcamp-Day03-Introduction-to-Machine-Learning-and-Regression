# Day 3 – Regression: Car Price Prediction

## Overview
This notebook explores regression algorithms and develops machine learning models to predict car prices from vehicle characteristics. The goal was to achieve an **R² score above 0.85**.

## Objectives
- Load data from SQLite, JSON, and Excel files.
- Perform exploratory data analysis (EDA) and data visualization.
- Investigate relationships between numerical features and car prices.
- Check missing values and explore statistical significance using p-values.
- Examine outliers and perform feature engineering.
- Train and evaluate regression models.
- Compare models using **R²** and **Root Mean Squared Error (RMSE)**.
- Inspect residuals and explore data normalization.

## Workflow
1. **Data loading:** Read car data from different file formats.
2. **EDA:** Review dataset structure, summary statistics, distributions, and correlations.
3. **Visualization:** Use Seaborn and Matplotlib to explore patterns in the data.
4. **Feature selection and preparation:** Select features and encode categorical variables with one-hot encoding.
5. **Train/test split:** Use an 80/20 split with `random_state=42`.
6. **Model training:** Train and compare several regression algorithms.
7. **Evaluation:** Compare R² and RMSE and inspect residuals.

## Models Compared
The notebook compares multiple algorithms, including:
- Linear Regression
- Ridge, Lasso, and Elastic Net
- Huber Regression and Bayesian Ridge
- Decision Tree and Extra Tree
- Random Forest
- Gradient Boosting and HistGradientBoosting
- AdaBoost
- XGBoost
- CatBoost
- K-Nearest Neighbors (KNN)
- Support Vector Regression (SVR and NuSVR)
- Kernel Ridge
- Multi-layer Perceptron (MLP)

## Results
**CatBoost achieved the best result in the notebook's model comparison.**

| Metric | CatBoost result |
|---|---:|
| R² score | 0.995453 (approximately 99.55%) |
| RMSE | Approximately 360,625 |

The target R² score of **0.85 (85%)** was exceeded in this evaluation.

> **Note:** R² is not the same as classification accuracy. An R² score of 0.995453 indicates that the model explains approximately 99.55% of the variance in the test target for this particular split. The result should be validated with appropriate cross-validation and checks for data leakage before being treated as a reliable estimate of real-world performance.

## Tools and Libraries
- Python
- Pandas
- SQLite
- Matplotlib
- Seaborn
- scikit-learn
- XGBoost
- CatBoost
- Jupyter Notebook

## Key Takeaways
- Regression models estimate continuous values, such as vehicle prices.
- EDA and domain knowledge help guide feature selection.
- R² and RMSE provide complementary information about model performance.
- Residual analysis helps assess prediction errors.
- Comparing several algorithms can help identify a strong candidate model.

## Project Goal
Learn regression techniques and build a model that predicts car prices, with a target R² score above 85%.
