# 🏡 Housing Price Prediction

## 📌 Project Overview

This project aims to **predict housing prices** based on demographic, geographic, and economic features of different locations. The dataset represents housing data from California, including attributes such as population, income levels, number of rooms, and proximity to the ocean.

The final goal is to build a **regression model** that accurately estimates the **median house value** for a given location.

---

## 📂 Dataset Information

The dataset consists of **18,565 rows and 10 columns**.

### **Features**

* **longitude**: Geographical coordinate (east–west).
* **latitude**: Geographical coordinate (north–south).
* **housing\_median\_age**: Median age of houses in the area.
* **total\_rooms**: Total number of rooms in all households within a block.
* **total\_bedrooms**: Total number of bedrooms in all households within a block. *(contains missing values)*
* **population**: Population living in the block.
* **households**: Number of households in the block.
* **median\_income**: Median income of households in the block (in 10,000s of USD).
* **ocean\_proximity**: Categorical variable indicating closeness to the ocean (e.g., `<1H OCEAN`, `INLAND`).

### **Target**

* **median\_house\_value**: Median house price in the block (USD).

---

## 🔎 Project Steps

1. **Data Exploration & Cleaning**

   * Handle missing values in `total_bedrooms`.
   * Encode categorical feature `ocean_proximity`.
   * Feature scaling for numerical variables.

2. **Feature Engineering**

   * Create additional features like `rooms_per_household`, `bedrooms_per_room`, and `population_per_household`.

3. **Exploratory Data Analysis (EDA)**

   * Visualize distributions of target and predictors.
   * Correlation heatmap for numerical features.
   * Scatterplots of target vs. important features.

4. **Modeling**

   * Train baseline models: Linear Regression, Ridge, Lasso.
   * Train advanced models: Random Forest, Gradient Boosting (XGBoost, LightGBM).
   * Hyperparameter tuning using GridSearchCV/RandomizedSearchCV.

5. **Evaluation**

   * Metrics: RMSE, MAE, R² score.
   * Compare performance across models.
   * Select best-performing model for final recommendation.

---

## 🎯 Goal

The main objective is to **predict the median house value** for each location given the available features.
This model can be used for:

* Real estate market analysis.
* Assisting buyers/sellers in price estimation.
* Supporting policymakers in housing development strategies.

---

Would you like me to also add a **“How to Run” section** with Colab commands (mount Drive, run preprocessing, train model) so it looks like a complete project README?
