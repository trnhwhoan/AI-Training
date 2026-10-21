# AI-Training

## Book: Grokking Machine Learning
## Day 3

### Train/Test Split & Overfitting
#### Why is it necessary to split data?
- Split data is to verify whether a model has truly learned the underlying patterns to make predictions on new data, or if it has simply memorized the data it was trained on.
- ex: Glowee have data of 1000 customers and want to forecast level of spending next month.
  -- 1000 customers -- 800 **Training Set** (have the model learn from data and answers) + 200 **Test Set** (check the model using unseen data).
- Training Set and Test Set
|  | Training Set | Test Set |
| :--- | :---: | ---: |
| Purpose | training the model | rating on data unseen to learn |
| Is the model trained on data? | Yes | No |
| Have real labels? | Yes, in supervised learning | Yes, for the purpose of comparing predictions |
| Using time | Training | After training |

#### What is Overfitting?
- **Overfitting** occurs when a model learns the training data too closely—including noise—which results in poor predictive performance on new data.
- ex: Glowee have 100 customers have purchased cosmetics. And we have a model to predict whether those 100 customers will make another purchase next month.
  <img width="615" height="266" alt="image" src="https://github.com/user-attachments/assets/51f617cb-3501-4ab4-93cf-d30739a4cb34" />
-- **Underfitting** - The model too simple or insufficiently trained, resulting in poor performance even on the training data.
-- **Good Fit** - The model that has learned the underlying patterns is capable of generalizing to new data.
-- **Overfitting** - The model overfits the training data but performs poorly when making predictions on new data.

#### Data Leakage
- **Data Leakage** is a error that AI Engineers must be careful. Specifically, this refers to a phenomenon where a model inadvertently gains access to information from the validation set, test set, or future data during the training process—resulting in high evaluation metrics (such as accuracy or AUC) on paper, while failing when deployed in real-world scenarios.
- ex: Glowee want to forecast whether the customer will make a purchase in November.
  -- **Valid features**: Number of orders up tho the end of October, total expenditure incurred before November, and number of visits prior to the prediction timeframe.
  -- **Invalid feature**: Number of orders actually placed by customers in November.
- In forecast time, future information does not yet exist. When used for training, the model might achieve a very high score, yet fail to function properly in real-world scenarios.
- **Use only information that is actually available at the time the prediction is made.**

**High Training Accuracy + Low Test Accuracy → Suspect Overfitting, Investigate Further.**
  
