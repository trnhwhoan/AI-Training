# AI-Training

## Book: Grokking Machine Learning
## Day 2

### Models, Training & Prediction
#### Machine Learning Model
##### Models
- **Model** - a *Machine Learning Model* is a math model of caculate have parameters learned from data, to identify patterns and make predictions.
- ex: Want to prediction base on learn time
<img width="446" height="232" alt="image" src="https://github.com/user-attachments/assets/c992c7a7-8eb9-4535-94cd-56ed4380e54e" />

   -- The rule of table: y = 10x + 30
  -- If learn time is 6 hours, the model can prediction: y = 10(6) + 30 = 90
  --> **Linear Regression**

##### What is the difference between training and prediction?
- **Training** - the model use data with answers to studies parameters and rule.
- **Prediction** - the model studied use features to prediction output value.
<img width="557" height="224" alt="image" src="https://github.com/user-attachments/assets/f4b48fa0-0aa6-4df2-9e11-821673d01a8a" />

##### How does the model learn?
- Step 1: Model show prediction base on these present parameters.
- Step 2: Compare prediction with truth answers.
- Step 3: Calculate errors by **loss function**
- Step 4: Find ways to adjust parameters to reduce errors.
- The specific process depends on the algorithm.
- ex: Linear Regression can find parameters by least squares method, different Gradient Descent.
  -- y = wx + 30


- Formula for calculating Absolute Error (AE):
  <img width="247" height="51" alt="image" src="https://github.com/user-attachments/assets/f66be0c8-139f-498e-a095-039c30da7e02" />


 





