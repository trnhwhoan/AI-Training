# AI-Training

## Book: Grokking Machine Learning
## Week 3 - Day 7

### Review & Mini Project
#### Objective
Build and compare regression models to predict diabetes progression using the Scikit-learn Diabetes dataset.

#### Dataset
- Samples: 442
- Features: 10
- Training samples: 353
- Testing samples: 89

#### Models
- Linear Regression
- Ridge Regression (L2)
- Lasso Regression (L1)

#### Evolution Metrics
- MAE
- MSE
- R^2 Score

#### Results

| Model | MAE | MSE | R² Score |
|:---|---:|---:|---:|
| Linear Regression | 42.7941 | 2900.1936 | 0.4526 |
| Ridge Regression | 42.9969 | 2856.4869 | 0.4609 |
| Lasso Regression | 42.8318 | 2878.5594 | 0.4567 |


#### Conclusion
Ridge Regression achieved the lowest MSE and highest R² score among the three tested models, while Linear Regression achieved the lowest MAE.

The results show that regularization can improve some evaluation metrics, but it does not necessarily outperform the baseline model in every metric.



















  
