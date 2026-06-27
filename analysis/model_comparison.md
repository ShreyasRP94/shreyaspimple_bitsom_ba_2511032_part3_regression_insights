# Model Comparison

## Overview

Four regression models were developed to identify the factors influencing monthly sales. Three simple linear regression models evaluated the impact of individual predictors, while one multiple regression model examined the combined effect of all predictors.

| Model                                        | Dependent Variable | Independent Variable(s)                                                        |        R² | Significant Variables (p < 0.05)                  | Business Usefulness                                                                                                                                    | Limitations                                                                                                                                                                                                 |
| -------------------------------------------- | ------------------ | ------------------------------------------------------------------------------ | --------: | ------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Model 1: Sales vs Marketing Spend**        | Monthly Sales      | Marketing Spend                                                                | **0.167** | Marketing Spend (p < 0.001)                       | Shows that marketing investment has a statistically significant positive impact on sales. Useful for evaluating marketing effectiveness.               | Explains only 16.7% of sales variation. Ignores other important drivers such as customer traffic and inventory availability.                                                                                |
| **Model 2: Sales vs Footfall**               | Monthly Sales      | Footfall                                                                       | **0.736** | Footfall (p < 0.001)                              | Strong predictor of sales. Indicates that customer traffic is the primary driver of monthly sales. Useful for forecasting sales and store performance. | Does not account for marketing efforts, inventory availability or store characteristics.                                                                                                                    |
| **Model 3: Sales vs Inventory Availability** | Monthly Sales      | Inventory Availability (%)                                                     | **0.013** | Inventory Availability (p = 0.0406)               | Inventory availability has a statistically significant positive relationship with sales.                                                               | Very low explanatory power (1.3%). Inventory alone is insufficient to predict sales and should not be used independently.                                                                                   |
| **Model 4: Multiple Regression Model**       | Monthly Sales      | Marketing Spend, Footfall, Inventory Availability (%), High Street Store Dummy | **0.805** | Marketing Spend, Footfall, Inventory Availability | Provides the highest predictive accuracy by combining multiple business drivers. Suitable for forecasting and business planning.                       | High Street store dummy is not statistically significant (p = 0.890). The model also does not capture other external factors such as pricing, promotions, competition, seasonality and economic conditions. |

---

# Comparison of Model Performance

The simple regression model using **Marketing Spend** explains only **16.7%** of the variation in monthly sales, indicating that although marketing investment contributes positively to sales, it is not the primary driver.

The **Footfall** model performs substantially better, explaining **73.6%** of the variation in sales. This demonstrates that customer traffic is the strongest individual predictor of monthly sales.

The **Inventory Availability** model has the weakest explanatory power with an R² of only **1.3%**. Although the relationship is statistically significant, inventory availability alone contributes very little to explaining sales variation.

The **Multiple Regression Model** achieves the highest explanatory power with an **R² of 80.5%**, indicating that combining multiple predictors provides a much better explanation of sales performance than relying on any single variable.

---

# Significant Variables

The multiple regression model shows:

* **Marketing Spend** is statistically significant (p < 0.001).
* **Footfall** is highly statistically significant (p < 0.001) and is the strongest predictor of sales.
* **Inventory Availability (%)** is statistically significant (p < 0.001) after controlling for the other variables.
* **High Street Store Dummy** is **not statistically significant** (p = 0.890), suggesting that after accounting for marketing spend, footfall and inventory availability, store type does not have a meaningful additional impact on monthly sales.

---

# Business Recommendation

Among all four models, the **Multiple Regression Model** is recommended for business decision-making because it explains approximately **80.5%** of the variation in monthly sales.

The analysis suggests that increasing customer footfall, investing appropriately in marketing and maintaining higher inventory availability are the most effective levers for improving sales.

Since the High Street store dummy is not statistically significant, store location type alone should not be considered a major determinant of sales within this dataset.

---

# Overall Conclusion

The multiple regression model provides the best balance between explanatory power and business insight. While footfall is the strongest individual predictor, combining marketing spend and inventory availability further improves prediction accuracy. Future models could be enhanced by including additional variables such as product pricing, promotional campaigns, seasonality, competitor activity and local economic conditions.
