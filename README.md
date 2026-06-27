# shreyaspimple_bitsom_ba_2511032_part3_regression_insights

# Sales Regression Analysis

## Business Problem Summary

A retail company wants to understand the key factors influencing monthly store sales. While several operational and marketing metrics are tracked, management needs evidence-based insights into which variables have the strongest relationship with sales and which business levers should be prioritised.

The objective of this project is to use linear regression analysis to quantify the relationship between monthly sales and key business variables, compare different regression models, and recommend the most suitable model for business decision-making.

---

# Dataset Description

The dataset contains monthly operational data for multiple retail stores over four months. Each record represents the performance of one store during a specific month.

The dataset includes:

* Store ID
* Month
* Monthly Sales
* Marketing Spend
* Footfall
* Inventory Availability (%)
* Store Type
* Other store-level attributes

Each Store ID appears multiple times because the dataset contains monthly observations rather than duplicate records.

---

# Dependent and Independent Variables

### Dependent Variable

* **Monthly Sales**

### Independent Variables

* Marketing Spend
* Footfall
* Inventory Availability (%)
* Store Type (converted into a dummy variable)

---

# Regression Approach

The analysis was completed in several stages:

1. Performed exploratory data analysis and checked data quality.
2. Created a dummy variable for the categorical Store Type variable.
3. Developed three simple linear regression models:

   * Sales vs Marketing Spend
   * Sales vs Footfall
   * Sales vs Inventory Availability
4. Built a multiple linear regression model using all independent variables.
5. Compared model performance using R² values and statistical significance.
6. Performed residual analysis to evaluate prediction accuracy.
7. Selected the best-performing model based on explanatory power and business usefulness.

---

# Dummy Variable Approach

Store Type is a categorical variable and therefore cannot be directly included in a regression model.

A dummy variable was created as follows:

| Store Type      | High_Street_Dummy |
| --------------- | ----------------: |
| High Street     |                 1 |
| Non-High Street |                 0 |

The **Non-High Street** category was used as the reference category.

This approach allows the regression model to estimate whether High Street stores perform differently from other store types while controlling for the remaining variables.

---

# Model Comparison Summary

Four regression models were evaluated.

| Model               | Independent Variables                                                    |         R² | Key Findings                                                                                                                                                                      |
| ------------------- | ------------------------------------------------------------------------ | ---------: | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Simple Regression   | Marketing Spend                                                          | **0.1672** | Marketing spend has a significant positive relationship with sales but explains only a small proportion of variation.                                                             |
| Simple Regression   | Footfall                                                                 | **0.7363** | Footfall is the strongest individual predictor of monthly sales.                                                                                                                  |
| Simple Regression   | Inventory Availability (%)                                               | **0.0131** | Inventory availability is statistically significant but has very low explanatory power when analysed alone.                                                                       |
| Multiple Regression | Marketing Spend, Footfall, Inventory Availability (%), High Street Dummy | **0.8046** | Best-performing model with the highest explanatory power. Marketing Spend, Footfall and Inventory Availability are statistically significant, while the High Street dummy is not. |

---

# Final Model Selected

The **Multiple Linear Regression Model** was selected as the final model because it achieved the highest explanatory power (**R² = 0.8046**) and explained approximately **80.5%** of the variation in monthly sales.

The final model incorporates multiple business drivers simultaneously, providing more accurate predictions and more practical business insights than the individual regression models.

---

# Business Recommendation

Based on the regression analysis, the following recommendations are made:

* Prioritise initiatives that increase customer footfall, as it is the strongest predictor of monthly sales.
* Continue investing strategically in marketing activities that drive customer visits and improve sales performance.
* Maintain high inventory availability to minimise lost sales opportunities caused by stock shortages.
* Monitor stores with consistently large residuals to identify operational best practices or underlying performance issues.
* Do not make strategic decisions based solely on store type, as the High Street dummy variable was not statistically significant in the final model.

---

# Assumptions and Limitations

### Assumptions

* Linear relationships exist between the dependent and independent variables.
* Observations are independent.
* Residuals are approximately normally distributed.
* Variance of residuals is relatively constant across observations.
* Multicollinearity among predictors is minimal.

### Limitations

* Approximately **19.5%** of sales variation remains unexplained by the final model.
* Important business factors such as pricing, promotions, competitor activity, holidays, weather and customer demographics were not included in the analysis.
* Regression identifies statistical associations but does not establish causal relationships.
* The model is based on historical data and may not fully predict future market conditions.

---

# Screenshots Included

The repository includes screenshots supporting the analysis, including:

* Simple regression outputs
* Multiple regression output
* Residual analysis
* Regression models comparison tables

These screenshots provide visual evidence of the statistical analysis and support the findings presented in this project.

---

# Project Summary

This project demonstrates how regression analysis can be used to support business decision-making by identifying the key drivers of monthly sales. The analysis found that **customer footfall**, **marketing spend**, and **inventory availability** are the most important factors associated with sales performance. The multiple regression model provided the strongest predictive capability and forms the basis of the final business recommendations.
