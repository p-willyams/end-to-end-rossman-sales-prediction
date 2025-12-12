
<img width="1920" height="1080" alt="PATRYCK WILLYAMS(3)" src="https://github.com/user-attachments/assets/8b367eb6-c8ce-4445-8bba-a304fd490b80" />
Below is a complete **English README** in the *same structure, tone, formatting, and level of detail* as the example you provided — but fully adapted to your **Rossmann Sales Forecasting Project**.

# Rossmann Sales Forecasting — End-to-End Predictive Model

## Project Overview

This project focuses on developing a **predictive model to estimate store sales for the next six weeks** across a large pharmacy retail chain (Rossmann). The objective is to support **strategic investment decisions**, such as renovations, expansion, inventory planning, and marketing campaigns, by identifying which stores have the highest potential return.

The model was built using historical sales data, store characteristics, promotional activity, and temporal information, applying Data Science and Machine Learning techniques to deliver accurate and actionable forecasts.

---

## Business Problem

Store managers were manually forecasting sales—a process highly inconsistent due to factors such as promotions, seasonality, competition, regional effects, and holidays. The business needed:

* Consistent and reliable **short-term sales forecasts**
* Insight into **which stores are most profitable to invest in**
* Understanding of **temporal patterns** and seasonal behavior
* A scalable, automated system to support **data-driven decision-making**

---

## Solution

A **regression model** was developed to predict six-week sales for more than 3,000 Rossmann stores across several European countries.

The workflow included:

* Exploratory Data Analysis (EDA)
* Feature engineering (temporal variables, promotion flags, store characteristics, seasonality indicators)
* Attribute selection
* Training and validation of multiple models
* Deployment via API and automated pipeline

After testing several algorithms, the **XGBoost Regressor** delivered the best balance between accuracy, computational efficiency, and generalization.

---

## Model Performance

| Metric   | Value     |
| -------- | --------- |
| **R²**   | **0.89**  |
| **MAPE** | **9.6%**  |
| **RMSE** | **1,010** |
| **MAE**  | **684**   |

These results demonstrate that the model captures most of the variance in sales and can be reliably used for strategic planning.

---

## Business Interpretation

The analysis revealed that sales performance is influenced not only by structural store characteristics but largely by **temporal and seasonal patterns**, such as:

* Time of year
* Holiday periods
* Weekly sales behavior
* Long-term downward trends

With this model, store owners can:

* Identify units with the **highest investment potential**
* Plan **promotional campaigns** during periods of high demand
* Avoid investing in low-return periods or locations
* Monitor long-term behavioral trends across stores

---

## Error Analysis per Store

The model performs consistently for most stores, with **MAPE typically between 3% and 10%**, which is excellent for retail forecasting.
Some stores exhibit higher variability and were more difficult to predict (e.g., Store 909 with MAPE ~36%), likely due to irregular events, unobserved promotions, or atypical behavior.

Understanding these edge cases helps improve:

* Model robustness
* Data quality checks
* Local business insights

---

## Forecasting Scenarios

| Scenario            | Value           |
| ------------------- | --------------- |
| **Predicted sales** | $270,079,776.00 |
| **Worst case**      | $254,067,448.02 |
| **Best case**       | $286,092,126.34 |

These scenarios help decision-makers evaluate risks, budget allocation, and strategic planning.

---

## Model Diagnostics

The evaluation plots demonstrate:

1. **Real vs. Predicted Sales**

   * Strong alignment between curves
   * Accurate modeling of peaks and seasonal drops

2. **Error Rate Over Time**

   * Balanced errors with no systemic bias

3. **Error Distribution**

   * Symmetric and centered near zero, indicating no over- or underestimation trend

4. **Error vs. Prediction**

   * Stable performance across the entire prediction range

The model generalizes well and is suitable for production use.

---

## Data Source

The dataset contains **daily sales records** for thousands of Rossmann stores across seven European countries, including information on:

* Store type
* Promotions
* Competition
* Assortment
* Holidays
* School holidays
* Temporal patterns

---

## Conclusion

This project successfully delivered a **robust and scalable predictive model** capable of estimating six-week sales across the Rossmann store network. Key outcomes:

* Reliable, high-accuracy forecasts (MAPE ≈ 9.6%)
* Automated scoring pipeline and production-ready API
* Support for strategic decisions regarding investment, marketing, and expansion
* Clear insights into temporal behavior and long-term trends
* Identification of stores with high or low forecast reliability

Overall, the project demonstrates the practical value of **Data Science and Machine Learning** in a real business environment, transforming historical data into **actionable insights** and enabling more assertive decision-making.
