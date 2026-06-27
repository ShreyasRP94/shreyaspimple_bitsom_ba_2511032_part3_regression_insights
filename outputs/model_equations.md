# Model Equations

## Overview

Four regression models were developed to evaluate the relationship between monthly sales and different business variables. Three simple linear regression models assessed the individual impact of marketing spend, footfall and inventory availability, while one multiple regression model evaluated their combined effect along with store type.

---

# 1. Simple Regression Model: Sales vs Marketing Spend

### Regression Equation

```text
Sales = 560,777.3454 + 2.1296 × Marketing Spend
```

### Business Interpretation

* **Intercept (560,777.35):** Represents the estimated monthly sales when marketing spend is zero. Although this situation is unlikely in practice, it provides the baseline level of sales.
* **Marketing Spend Coefficient (2.1296):** For every additional **₹1** invested in marketing, monthly sales are expected to increase by approximately **₹2.13**, on average.

This model demonstrates that marketing investment has a positive impact on sales, although it explains only **16.7%** of the variation in sales.

---

# 2. Simple Regression Model: Sales vs Footfall

### Regression Equation

```text
Sales = 446,410.5829 + 35.6780 × Footfall
```

### Business Interpretation

* **Intercept (446,410.58):** Represents the estimated monthly sales when customer footfall is zero.
* **Footfall Coefficient (35.6780):** Holding all else constant, every additional customer visiting the store is associated with an average increase of approximately **₹35.68** in monthly sales.

Among the simple regression models, footfall is the strongest predictor of sales, explaining **73.6%** of the variation in monthly sales.

---

# 3. Simple Regression Model: Sales vs Inventory Availability

### Regression Equation

```text
Sales = 484,814.2566 + 2,217.8319 × Inventory Availability (%)
```

### Business Interpretation

* **Intercept (484,814.26):** Represents the estimated baseline monthly sales when inventory availability is zero.
* **Inventory Availability Coefficient (2,217.8319):** A one percentage-point increase in inventory availability is associated with an increase of approximately **₹2,218** in monthly sales.

Although inventory availability has a statistically significant positive relationship with sales, this model explains only **1.3%** of the variation in sales, indicating that inventory availability alone is not a strong predictor.

---

# 4. Multiple Regression Model (Final Model)

### Regression Equation

```text
Sales =
135,188.3955
+ 1.1765 × Marketing Spend
+ 33.6906 × Footfall
+ 2,919.7025 × Inventory Availability (%)
+ 750.5427 × High Street Store Dummy
```

---

# Explanation of Each Coefficient

### Intercept (135,188.3955)

Represents the estimated monthly sales when all predictor variables are zero. While this scenario is not realistic, it serves as the starting point of the regression equation.

### Marketing Spend (1.1765)

Holding all other variables constant, every additional **₹1** spent on marketing is associated with an increase of approximately **₹1.18** in monthly sales.

### Footfall (33.6906)

Holding all other variables constant, every additional customer visiting the store is expected to increase monthly sales by approximately **₹33.69**.

Footfall is the strongest contributor to sales and has the highest statistical significance among all predictors.

### Inventory Availability (%) (2,919.7025)

Holding other variables constant, a one percentage-point increase in inventory availability is associated with an increase of approximately **₹2,920** in monthly sales.

This indicates that maintaining product availability positively influences store sales.

### High Street Store Dummy (750.5427)

After accounting for marketing spend, footfall and inventory availability, High Street stores are estimated to generate approximately **₹751** higher monthly sales than the reference store category.

However, this variable has a **p-value of 0.890**, indicating that the difference is **not statistically significant**. Therefore, store type does not provide meaningful additional explanatory power in this model.

---

# Explanation of Dummy Variable

A dummy variable was created to represent store type.

| Store Type      | High_Street_Dummy |
| --------------- | ----------------: |
| High Street     |                 1 |
| Non-High Street |                 0 |

The dummy variable allows the regression model to compare High Street stores with all other store types while keeping the remaining variables constant.

---

# Reference Category Used

The reference category is:

**Non-High Street Stores (High_Street_Dummy = 0)**

The coefficient of the dummy variable measures the difference in sales between High Street stores and this reference category.

---

# Final Model Selected

The **Multiple Regression Model** was selected as the final model.

---

# Reason for Selecting the Final Model

The multiple regression model was selected because it provides the most comprehensive explanation of monthly sales performance.

Compared with the individual regression models, it has the highest explanatory power with an **R² of 80.46%**, meaning that approximately **80.5%** of the variation in monthly sales is explained by the combined effect of marketing spend, customer footfall, inventory availability and store type.

The model also shows that:

* **Marketing Spend** is a statistically significant contributor to sales (**p < 0.001**).
* **Footfall** is the strongest and most significant driver of sales (**p < 0.001**).
* **Inventory Availability** is also a statistically significant predictor (**p < 0.001**).
* **High Street Store Dummy** is **not statistically significant (p = 0.890)**, indicating that store type does not meaningfully influence sales after accounting for the other variables.

From a business perspective, the analysis indicates that increasing customer footfall, investing effectively in marketing and maintaining high inventory availability are the primary levers for improving monthly sales. Therefore, the multiple regression model is the most suitable model for sales forecasting and business decision-making.
