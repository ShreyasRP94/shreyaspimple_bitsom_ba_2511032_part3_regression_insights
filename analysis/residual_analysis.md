# Residual Analysis

## Overview

Residual analysis was performed using the selected **Multiple Linear Regression Model**, where Monthly Sales is predicted using:

* Marketing Spend
* Footfall
* Inventory Availability (%)
* High Street Store Dummy

Predicted sales were calculated using the regression equation, and residuals were computed as:

**Residual = Actual Monthly Sales − Predicted Monthly Sales**

A positive residual indicates that actual sales exceeded the model prediction, while a negative residual indicates that actual sales were lower than predicted.

---

# Predicted Sales and Residual Calculation

The predicted sales values were generated using the final multiple regression equation:

```text
Predicted Sales =
135188.3955
+ 1.1765(Marketing Spend)
+ 33.6906(Footfall)
+ 2919.7025(Inventory Availability %)
+ 750.5427(Store_d)
```

Residuals were then calculated as:

```text
Residual = Actual Sales − Predicted Sales
```

Interpretation:

* Positive Residual → Model under-predicted sales.
* Negative Residual → Model over-predicted sales.
* Residual close to zero → Accurate prediction.

---

# Five Largest Positive Residuals (Model Under-predicted)

| Rank | Observation | Predicted Sales |       Residual |
| ---: | ----------: | --------------: | -------------: |
|    1 |         112 |      601,880.79 | **111,730.37** |
|    2 |         104 |      523,384.40 | **102,129.64** |
|    3 |         202 |      687,300.86 | **100,414.65** |
|    4 |         125 |      815,816.68 |  **98,727.49** |
|    5 |         254 |      702,290.08 |  **96,756.86** |

### Business Interpretation

These observations generated substantially higher sales than predicted by the regression model. Possible explanations include:

* Successful local marketing campaigns not captured in the dataset.
* Better customer conversion rates.
* Superior store management or customer service.
* Product mix or merchandising advantages.
* Seasonal or local events increasing demand.

These residuals indicate that additional variables influencing sales are not currently included in the model.

---

# Five Largest Negative Residuals (Model Over-predicted)

| Rank | Observation | Predicted Sales |        Residual |
| ---: | ----------: | --------------: | --------------: |
|    1 |          67 |      842,714.80 | **-157,335.72** |
|    2 |          45 |      729,410.26 | **-133,942.66** |
|    3 |          33 |      760,303.73 | **-118,438.70** |
|    4 |           4 |      773,539.56 | **-114,619.26** |
|    5 |          90 |      737,656.42 | **-110,484.52** |

### Business Interpretation

These observations recorded considerably lower sales than predicted by the model. Possible reasons include:

* Temporary operational issues or store closures.
* Product stock-outs despite adequate overall inventory levels.
* Increased local competition.
* Poor customer experience or staffing issues.
* External factors such as weather or regional events reducing demand.

These cases suggest that some store-specific or external factors affecting sales are not represented in the current regression model.

---

# Does the Model Under-Predict or Over-Predict Certain Stores?

The multiple regression model explains approximately **80.5%** of the variation in monthly sales (R² = 0.805), indicating a strong overall fit.

Residual analysis shows that:

* Observations with **large positive residuals** indicate cases where the model under-predicted sales.
* Observations with **large negative residuals** indicate cases where the model over-predicted sales.

There is **no evidence that the model systematically under-predicts or over-predicts High Street stores**, since the High Street dummy variable was **not statistically significant (p = 0.890)** in the final model.

Instead, the largest prediction errors are more likely due to variables not included in the model, such as promotional campaigns, pricing strategies, competitor activity, local demographics, seasonal demand, and weather conditions.

---

# Overall Assessment

The selected multiple regression model provides a good fit and explains approximately **80.5%** of the variation in monthly sales. While predictions are generally accurate, the largest residuals highlight that additional business factors influence store performance beyond marketing spend, footfall, inventory availability, and store type.

Including variables such as promotions, pricing, holidays, local competition and customer demographics could further improve the predictive performance of the model.
