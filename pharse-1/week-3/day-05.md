# AI-Training

## Book: Grokking Machine Learning
## Week 3 - Day 5

### Training First ML Model
#### Review

- *Model Training* - process of model learning relationships between Feature (input) and Labels (output) from training data.

- *.fit()* - method use to train model

model.fit(X_train, y_train)

In there:

- model -- Machine Learning model
  
- X_train -- input data
  
- y_train -- corresponding actual results

- *Intercept & Coefficients* - after trining Linear Regression, can watch:
  
  - model.intercept_: bias
    
  - model.coef_: weights corresponding with features.

- *.predict()* - use trained model to predict new data.

predictions = model.predict(X_test)


















  
