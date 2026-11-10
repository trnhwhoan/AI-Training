# AI-Training

## Book: Grokking Machine Learning
## Week 3 - Day 2

### Loss Function & MSE
#### Why does a model need a Loss Function?
- At day 01, Linear Regression = y(hat) = wx + b

But, how can you tell whether a predictive model is good or bad?

ex: Glowee have reality data:

| Visits | Reality revenue |
| --- | --- |
| 100 | 500.000đ |
| 200 | 900.000đ |
| 300 | 1.300.000đ |

- Suppose the model predicts a revenue of 450,000 VND when there are 100 visits.
  
  -- Reality: 500.000đ

  -- Prediction: 450.000đ

  -- Deviation: 50.000đ

- The gap between the predicted value and the actual value is the **Error**

  **Error** = *y - y(hat)*

    -- *y*: actual value

    -- *y(hat)*: prediction value

#### What is Loss Function?
- **Loss Function** is function use to measure the degree of discrepancy between the model's predictions and the actual data.
  
- Typically, the model attempts to find the parameters *w* and *b* that minimize the loss.
  
- The smaller the loss, the closer the predictions are to the actual values.

#### Mean Squared Error (MSE)
- MSE is a common way to measure error in Linear Regression.

  <img width="228" height="80" alt="image" src="https://github.com/user-attachments/assets/fcb67baa-7db2-4c64-91fd-64c50a044921" />

    -- *n*: number of data samples.

    -- *y_i*: actual value of the \(i\)-th sample.

    -- *y(hat)_i*: predicted value of the \(i\)-th sample.

Squaring the errors ensures that positive and negative errors do not cancel each other out.

Dividing by *n* yields the average.

ex: Suppose the model predicts 3 orders for Glowee:


| Oders | Actual | Prediction | Error |
| --- | --- | --- | --- |
| 1 | 500 | 450 | 50 |
| 2 | 900 | 1.000 | -100 |
| 3 | 1.300 | 1.200 | 100 |

<img width="291" height="234" alt="image" src="https://github.com/user-attachments/assets/ce4478a9-e9e0-42c8-a173-7672f9c6be3a" />

*Note: MSE is expressed in squared units, so it cannot be interpreted directly as the magnitude of the error.


