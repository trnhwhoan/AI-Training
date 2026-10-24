# AI-Training

## Book: Grokking Machine Learning
## Day 5

### Training Your First ML Model
#### Theory — How does Linear Regression work?
- At day 02, we have: y = wx + b
- For multiple features, the general formula is:

<img width="316" height="33" alt="image" src="https://github.com/user-attachments/assets/4d2f01d5-2907-41b8-9e93-86b53e7a5e23" />

- In Diabetes Dataset, model will learn 10 weights and a intercept from Training Set.
- ex: Glowee want to forecast spending level base on oder number before, with:

  <img width="379" height="42" alt="image" src="https://github.com/user-attachments/assets/2f5ee330-1a53-476d-b1da-8a39d092bc9f" />
  
  So, if oder number = 10, we have 150.000 x 10 + 100.000 = 1.600.000

#### fit ()
- When call **model.fit(X_train, y_train)** - Scikit-learn’s Linear Regression finds the coefficients (w_1,..,w_{10}) and (b) such that the sum of squared errors on the training set is minimized, using the ordinary least squares method.
- When call **model.predict(X_test)** - Model use the learned coefficients to calculate predicted values ​​for 89 samples in the Test Set.

| fit() | predict() |
|---|---|
| Learns model parameters | Uses learned parameters |
| Requires X_train and y_train | Requires input features X |
| Performs training | Performs inference |
| Produces a trained model | Returns predictions |



