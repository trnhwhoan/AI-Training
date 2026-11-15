# AI-Training

## Book: Grokking Machine Learning
## Week 3 - Day 4

### Regularization
#### What is Regularization?
- At day 3, Polynomial Regression drgree 15 model have:

  - Training MSE = 0.083330 - quite low
  - Testing MSE = 0.673715 - much higher

- This is Overfitting token: the model has learned the training data too closely, resulting in poor predictions on new data.

- **Regularization** is a technique that helps limit model complexity by adding a penalty term to the loss function.

- Two common methods: **Ridge Regression** & **Lasso Regression**
  
- **Ridge Regression (L2)**:
  
  - Penalizes the sum of the squared coefficients.
    
  - Shrinks the coefficients.
    
  - Typically does not drive coefficients exactly to zero.
    
  - Suitable when many features are useful.
 
  <img width="1864" height="1588" alt="image" src="https://github.com/user-attachments/assets/af41e016-47ef-4d18-b03d-283b7e4665cd" />

- **Lasso Regression (L1)**:

  - Applies a penalty based on the absolute values ​​of the numbers.

  - Can drive certain values ​​to zero.

  - Capable of automatically selecting filtering features.

  - Useful when a simpler model is desired.
 
    <img width="2126" height="1433" alt="image" src="https://github.com/user-attachments/assets/5e0251f5-3d03-4b24-9cf9-3e092391be28" />

**Formula**:

*Standard Linear Regression*:    *Loss* = *MSE*

*Ridge*: 

<img width="228" height="70" alt="image" src="https://github.com/user-attachments/assets/0a5a3499-dd56-459e-b370-c70c2ea3a855" />

*Lasso*:  

<img width="237" height="81" alt="image" src="https://github.com/user-attachments/assets/fea59bf9-9fa9-484b-9753-7dfc98b97eb6" />

In there:
- *MSE*: prediction error
- *w_j*: the coefficient of the j-th feature
- α (alpha): Regularization level

- **How does Alpha work?**
  
| Alpha | Impact |
| :--- | :---: |
| Small | Regularization low |
| Reasonable | Limit excessively large coefficients |
| Too big | The model maybe Underfitting |

*Regularization does not guarantee that a model will always perform better. We must still check the testing MSE to select an appropriate alpha value.*













  
