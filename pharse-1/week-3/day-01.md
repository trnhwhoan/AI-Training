# AI-Training

## Book: Grokking Machine Learning
## Week 3 - Day 1

### Linear Regression
#### What is Linear Regression?
- **Linear Regression** is a function Machine Learning can learn *linear relationship* between to input data with the result that needs to be predicted.

- We need to provide data for model learning. After, the model maybe predict result.

- ex: The model can predict revenue of Glowee base on daily website visits.

#### Formula
**y(hat) = wx + b**


| Ingredient | Meaning | ex of Glowee |
| --- | --- | --- |
| x | Input data | website visits  |
| w | weight | change in revenue per visit |
| b | bias | predict value when visits = 0  |
| y(hat) | prediction result | predict revenue |

ex: The model have: w = 4000; b = 100000

When visits is 250: y(hat) = 4000 x 250 + 100000 = 1.100.000

*Notes: In reality Machine Learning, *weight* and *bias* often to be taught form training data, instead of setting the data yourself.

- *Weight bigger*: When other factors remain constant, a change of one unit in an input will cause a larger change in the prediction.

- *Negative weight*: Input increase may lead to a decrease in the prediction.

- *Bias*: The predicted value when all inputs are equal to zero in a corresponding linear model.

  --**These are the parameters that directly influence the prediction result.**






