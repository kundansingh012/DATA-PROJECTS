# Prediction of International Education Cost

## Project Overview

This project helps international students estimate the **total cost of studying abroad**. Initially we applied basic data science techniques to clean and process the data by removing unnecessory data. We converted living cost index, rent etc. to total living cost and Rent_Total in USD. So that all values are in USD and gives data as per the program duration. We analyzed expenses like tuition, rent, living costs, visa cost, and insurance, using Linear regression as baseline model and polynomial regression for comparision.In addition, we used desicion tree to predict the total of the university programs. We have used univariate and bivariate analysis to check the relationship/ driving factors of toatl cost.

---

## Dataset Source

- **Title**: [Cost of International Education](https://www.kaggle.com/datasets/adilshamim8/cost-of-international-education/data)
- **File**: `International_Education_Costs.csv`
- **Source**: Kaggle
- **Description**: Contains data of different university from various countries, including tuition, rent, living cost index, visa fee, insurance, and exchange rate.

---

## Objectives

- We will use different cost components to predict the **total education cost**.
- To forecast toatl cost we use linear regression model.
- Cluster programs by affordability profiles.
- Parameter tuning and model comparison.
- Look up total cost by university name.

---

## Data Preparation & Exploration

- **Missing values handled**
- **Feature engineering**: `Living_Cost_Total`, `Rent_Total`, `Total_Cost`
- **Train/Validation/Test split**: 75/12.5/12.5
- **Scaling**: StandardScaler used for regression models
- **Univariate Analysis**: Distribution plots of cost features
- **Bivariate Analysis**: Scatter plots vs. `Total_Cost`, correlation heatmap

---

## Clustering Analysis

- **KMeans** clustering on top 3 cost drivers: `Tuition`, `Rent`, `Living_Cost`
- Visualised clusters in Tuition vs Total Cost space
- Cluster labels added to the dataset for optional model use
- silhouette score

---

## Models Used

| Model                    | Type        | Purpose           |
|--------------------------|-------------|-------------------|
| Linear Regression         | Baseline    | Simple benchmark  |
| Polynomial Regression     | Improved    | Captures non-linearity |
| Decision Tree Regressor  | Advanced  | Non-linear modeling |
| KMeans Clustering         | Exploratory | Affordability groups |

## Model Comparison: 
- Linear vs Polynomial Regression vs Decision Tree

## Residual Analysis – Model Error Diagnostics
---

## Parameter Tuning

- **Decision Tree `max_depth`** tuned from 2 to 10
- Optimal at `max_depth = 10`
- Evaluated using: R², MAE, MSE

---

## Evaluation Metrics

- **R² Score**
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Visuals**: Predicted vs Actual plots, Residual plots, Parameter vs Performance graphs

---

## Custom Feature: University Lookup Tool

Users can input a **university name** to retrieve:
- Predicted total education cost
- Associated affordability **cluster group**

---

## Results Summary

| Model               | R² Score | RMSE ($) | MAE ($) |
|---------------------|----------|----------|---------|
| Linear Regression   | 1.0000   | 0.00     | 0.00    |
| Polynomial Regression | 1.0000 | 0.00     | 0.00    |
| Decision Tree (Tuned) | 0.9919 | 3,603.92 | 2,369.87 |

---

## Requirement Checklist

| Requirement                                                | Status |
|-------------------------------------------------------------|--------|
| Define a meaningful objective and research questions        | ✅     |
| Perform data cleaning, preprocessing, and exploration       | ✅     |
| Use at least one baseline and one advance model             | ✅     |
| Compare model performance and justify decisions             | ✅     |
| Include visualisation and discussion of model results       | ✅     |

---

## Other Coverage

| Suggestion                                                                 | Status |
|----------------------------------------------------------------------------|--------|
| Linear Regression as baseline                                              | ✅     |
| Polynomial Regression to improve baseline                                 | ✅     |
| Use of clustering for structure discovery                                 | ✅     |
| Use of Decision Tree                                                      | ✅     |
| Parameter tuning on a model (Decision Tree `max_depth`)                  | ✅     |
| Evaluation with multiple metrics (MAE, MSE, R²)                            | ✅     |
| Optional function for user lookup by university name                      | ✅     |

---

## Technologies Used

- Python 3.11+
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
- Jupyter Notebook

---

## References

- [Scikit-learn Metrics Docs](https://scikit-learn.org/stable/modules/model_evaluation.html)
- [Kaggle Dataset Source](https://www.kaggle.com/datasets/adilshamim8/cost-of-international-education/data)

---

## Author

- Name: *Kundan Singh Shekhawat*

