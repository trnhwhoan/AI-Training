# AI-Training

## Book: Grokking Machine Learning
## Day 6

### Evaluating Your First ML Model
#### Warm-up
- A look back at the results from day 05:

| Sample | Actual | Predicted |
| --- | --- | --- |
| 0 | 219 | 139.55 |
| 1 | 70 | 179.55 |
| 2 | 202 | 134.04 |
| 3 | 230 | 291.42 |
| 4 | 111 | 123.79 |

-> Error0 = |219 - 139.55| = 79.45
-> Error1 = |70 - 179.52| = 109.52
=> Sample 0 predicted to be better sample 1, because *absolute error* smaller.
- However, if there are too many test samples, it becomes impossible to perform the calculations by hand; this is where **MAE** comes in.

### Mean Absolute Error (MAE)
- **MAE** is a metric used to assess the discrepancy between the predicted values ​​and the actual values ​​of a model.
$$
MAE = \frac{1}{n}\sum_{i=1}^{n}\left|y_i - \hat{y}_i\right|
$$
- In there:
  -- {n} - sample number evaluted
  -- y_i - acture value
  -- \hat{y}_i\ - model prediction value
  -- |y_i - \hat{y}_i\right| - absolute error of sample {i}

- ex: Glowee have prediction spending model for 3 customers:

| Customer | Actual | Predicted |
| --- | --- | --- |
| A | 500 | 450 |
| B | 800 | 900 |
| C | 300 | 250 |

-> MAE = $$ \frac{1}{3}\sum_{i=1}^{3}\left|500 - 450| $$


