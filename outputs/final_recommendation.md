# Final Recommendation

## Executive Summary

A series of regression models were developed to identify the business factors most strongly associated with monthly sales. After comparing three simple regression models and one multiple regression model, the **multiple regression model** was selected as the final model because it explains approximately **80.5% of the variation in monthly sales (R² = 0.8046)**. This provides the strongest overall explanation of sales performance among all models evaluated.

---

# Which Factors Appear Most Strongly Associated with Monthly Sales?

The regression analysis indicates that the following factors have the strongest association with monthly sales:

### 1. Customer Footfall (Strongest Driver)

Footfall is the most influential predictor of monthly sales.

* It produced the highest explanatory power among the simple regression models (**R² = 0.7363**).
* It remained highly statistically significant (**p < 0.001**) in the multiple regression model.
* The positive regression coefficient indicates that stores attracting more customers consistently generate higher sales.

**Business implication:** Increasing customer traffic should have the greatest impact on improving monthly sales.

---

### 2. Marketing Spend

Marketing spend has a positive and statistically significant relationship with monthly sales (**p < 0.001**).

Although marketing alone explains a relatively modest proportion of sales variation (**R² = 0.1672**), it remains an important contributor when combined with the other business variables.

**Business implication:** Well-targeted marketing investments can support higher sales by increasing customer awareness and store visits.

---

### 3. Inventory Availability

Inventory availability also has a positive and statistically significant relationship with monthly sales in the multiple regression model.

Stores with higher product availability are more likely to convert customer visits into completed purchases.

**Business implication:** Maintaining high inventory availability helps minimise lost sales opportunities and improves customer satisfaction.

---

# Which Variables Should Leadership Focus On?

Based on the regression evidence, leadership should prioritise the following areas:

* **Increasing customer footfall** through effective marketing campaigns, promotional events and customer engagement initiatives.
* **Optimising marketing expenditure** by investing in campaigns that deliver measurable increases in store traffic and sales.
* **Maintaining high inventory availability** to ensure products are consistently available when customers visit the store.

These three variables were statistically significant and collectively explain a substantial proportion of monthly sales performance.

---

# Which Variables Should Not Be Over-Interpreted?

The **High Street Store Dummy** should not be over-interpreted.

Although the regression coefficient suggests that High Street stores may generate slightly higher sales, the variable has a **p-value of 0.890**, indicating that the difference is **not statistically significant** after controlling for marketing spend, footfall and inventory availability.

This means there is insufficient statistical evidence to conclude that store type alone has a meaningful impact on monthly sales within this dataset.

Leadership should therefore avoid making strategic decisions solely based on store type.

---

# Recommended Business Actions

Based on the regression findings, the following actions are recommended:

1. **Increase customer footfall**

   * Strengthen local marketing campaigns.
   * Improve customer engagement programmes.
   * Enhance store visibility and promotional activities.

2. **Invest strategically in marketing**

   * Focus on marketing channels with measurable returns.
   * Continuously monitor campaign effectiveness using sales and customer traffic metrics.

3. **Maintain strong inventory management**

   * Improve demand forecasting.
   * Reduce stock-outs for high-demand products.
   * Ensure adequate inventory levels during peak sales periods.

4. **Monitor store performance continuously**

   * Compare actual sales against predicted sales.
   * Investigate stores with consistently large positive or negative residuals to identify operational best practices or underlying issues.

---

# Risks and Limitations

Although the final model performs well, several limitations should be considered when interpreting the results.

* Approximately **19.5% of the variation in monthly sales remains unexplained**, indicating that additional business factors influence sales.
* The model does not include variables such as pricing strategies, promotional discounts, competitor activity, seasonal demand, holidays, weather conditions or customer demographics.
* The High Street store dummy was not statistically significant and should not be interpreted as evidence that one store type consistently outperforms another.
* The regression model is based on historical data, and future market conditions may differ.

Leadership should therefore use the model as a decision-support tool rather than as the sole basis for strategic decisions.

---

# Why Regression Shows Association but Not Causation

Regression analysis identifies statistical relationships between variables, but it does **not automatically prove that one variable causes another**.

For example:

* Higher footfall is associated with higher sales, but the regression model cannot confirm that increasing footfall alone will always cause sales to increase.
* Similarly, higher marketing spend is associated with higher sales, but marketing expenditure may also be influenced by factors such as store performance, promotional strategies or seasonal campaigns.

Other unmeasured variables may simultaneously influence both the predictor variables and monthly sales.

Establishing causation would require additional methods such as controlled experiments, randomised trials or longitudinal studies.

Therefore, the findings from this regression analysis should be interpreted as evidence of **strong business associations**, rather than definitive proof of cause-and-effect relationships.

---

# Final Recommendation

The multiple regression model should be adopted as the primary analytical model for forecasting monthly sales because it provides the highest explanatory power (**R² = 0.8046**) and incorporates multiple significant business drivers.

The analysis indicates that **customer footfall is the strongest driver of sales**, supported by **marketing spend** and **inventory availability**. Leadership should prioritise initiatives that increase store traffic, optimise marketing investments and maintain high product availability.

At the same time, leadership should avoid over-interpreting the impact of **store type**, as it was not found to be a statistically significant predictor of sales. Future analyses should incorporate additional business variables to further improve the model's predictive accuracy and support more informed strategic decision-making.
