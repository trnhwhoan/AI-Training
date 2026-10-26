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


#### Mean Absolute Error (MAE)
- **MAE** is a metric used to assess the discrepancy between the predicted values ​​and the actual values ​​of a model.


MAE = (1/n) × Σᵢ₌₁ⁿ |yᵢ − ŷᵢ|

- In there:
  -- n - sample number evaluated
  
  -- y_i - acture value
  
  -- ŷᵢ - model prediction value
  
  -- |yᵢ − ŷᵢ| - absolute error of sample {i}

- ex: Glowee have prediction spending model for 3 customers:

| Customer | Actual | Predicted |
| --- | --- | --- |
| A | 500 | 450 |
| B | 800 | 900 |
| C | 300 | 250 |

-> MAE = (1/3) × Σ^3ᵢ₌₁ \ (|500-450|+|800-900|+|300-250|) ~ 66.67

**Notes**:
- MAE always not a negative number.
- MAE is lower, the smaller the mean absolute error.
- MAE = 0 -> exactly prediction
- MAE has the same units as the target.


#### Visualization
- If you calculate the average of the signed errors, the positive and negative errors may cancel each other out. MAE addresses this issue by taking the absolute value before calculating the average.
<img width="632" height="319" alt="image" src="https://github.com/user-attachments/assets/e5e4c7ed-b13d-403b-8d5e-2d4d5b8d7391" />

<img width="634" height="321" alt="image" src="https://github.com/user-attachments/assets/56c587a3-6961-4924-8c0d-12f3e9bad469" />

<img width="640" height="317" alt="image" src="https://github.com/user-attachments/assets/0afd61f6-27fe-45f5-9197-606327b35e63" />


**Notes** 
- Negative Signed Error: Predicted < Actual → The model’s prediction is lower than the actual value (Underprediction).

- Positive Signed Error: Predicted > Actual → The model’s prediction is higher than the actual value (Overprediction).

- Signed Error = 0: The prediction is equal to the actual value.






