# Model Equations

## Overview

Four regression models were developed to understand the factors influencing monthly sales. Three simple regression models evaluated the effect of individual business variables, while one multiple regression model assessed their combined impact.

---

# 1. Simple Regression Model: Sales vs. Marketing Spend

### Regression Equation

```text
Monthly Sales = 445,306.95 + 11.83 × Marketing Spend
```

### Business Interpretation

* The intercept (**445,306.95**) represents the estimated monthly sales when marketing spend is zero.
* The coefficient (**11.83**) indicates that for every additional **₹1** invested in marketing, monthly sales are expected to increase by approximately **₹11.83**, on average.
* This suggests that marketing investment positively influences sales, although it explains only a small proportion of the overall variation in sales.

---

# 2. Simple Regression Model: Sales vs. Footfall

### Regression Equation

```text
Monthly Sales = -79,564.36 + 429.73 × Footfall
```

### Business Interpretation

* The intercept (**−79,564.36**) has limited practical meaning because stores cannot realistically have zero customer visits.
* The coefficient (**429.73**) indicates that each additional customer visiting the store is associated with an increase of approximately **₹430** in monthly sales.
* Footfall is the strongest individual predictor of sales, explaining a large proportion of sales variation.

---

# 3. Simple Regression Model: Sales vs. Inventory Availability

### Regression Equation

```text
Monthly Sales = 386,145.52 + 2,648.74 × Inventory Availability (%)
```

### Business Interpretation

* The intercept (**386,145.52**) represents the estimated baseline monthly sales.
* The coefficient (**2,648.74**) indicates that improving inventory availability by **1 percentage point** is associated with an increase of approximately **₹2,649** in monthly sales.
* Although inventory availability has a positive effect on sales, its individual contribution to explaining sales variation is relatively small.

---

# 4. Multiple Regression Model (Final Model)

### Regression Equation

```text
Predicted Monthly Sales =
135,188.40
+ 1.1765 × Marketing Spend
+ 33.6906 × Footfall
+ 2,919.7025 × Inventory Availability (%)
+ 750.5427 × High Street Store Dummy
```

---

# Explanation of Each Coefficient

### Intercept (135,188.40)

Represents the estimated monthly sales when all predictor variables are zero. Although this situation is not realistic in practice, the intercept provides the baseline value for the regression equation.

### Marketing Spend (1.1765)

Holding all other variables constant, every additional **₹1** spent on marketing is associated with an average increase of approximately **₹1.18** in monthly sales.

### Footfall (33.6906)

Holding all other variables constant, each additional customer visiting the store is expected to increase monthly sales by approximately **₹33.69**.

### Inventory Availability (2,919.70)

Keeping other variables constant, a **1 percentage point** increase in inventory availability is associated with an increase of approximately **₹2,920** in monthly sales.

### High Street Store Dummy (750.54)

After controlling for marketing spend, footfall and inventory availability, High Street stores are estimated to generate approximately **₹751** higher monthly sales than the reference store category.

However, this coefficient is **not statistically significant (p = 0.890)**, indicating that store type does not have a meaningful independent impact on sales in this dataset.

---

# Explanation of Dummy Variable

A dummy variable was created to represent store type.

| Store Type         | High_Street_Dummy |
| ------------------ | ----------------: |
| High Street        |                 1 |
| Reference Category |                 0 |

The dummy variable allows the regression model to measure whether High Street stores perform differently from the reference store category while keeping all other variables constant.

---

# Reference Category Used

The reference category is the store type represented by **High_Street_Dummy = 0** (i.e., all non-High Street stores).

This category serves as the baseline against which High Street stores are compared.

---

# Final Model Selected

The **Multiple Regression Model** was selected as the final model for analysis.

---

# Reason for Selecting the Final Model

The multiple regression model was selected because it provides the most comprehensive explanation of monthly sales performance.

Compared with the three simple regression models, it achieved the highest explanatory power (**R² = 0.805**), indicating that it explains approximately **80.5%** of the variation in monthly sales.

The model combines multiple business drivers—marketing spend, customer footfall, inventory availability and store type—allowing sales to be predicted more accurately than models using a single variable.

Although the High Street dummy variable was not statistically significant, the overall model performed substantially better than the individual regression models.

From a business perspective, the analysis shows that customer footfall, effective marketing investment and maintaining high inventory availability are the primary factors associated with higher monthly sales. Therefore, the multiple regression model provides the most reliable foundation for forecasting sales and supporting operational decision-making.
