# CSGO-Round-Prediction
This project uses snapshots of each round to predict the winner of the round. The snapshot is recorded every 20 seconds from the round start until the round is decided. Each record contains information such as previous rounds' winner, remaining time of the round, each team's HP and equipment, etc. This dataset is obtained from: https://www.kaggle.com/datasets/christianlillelund/csgo-round-winner-classification

In the project, I trained and tuned a logistic regression model, a random forest model, and a shadow neural network model and compared their performance. Among them, random forest performs the best and achieves a test accuracy of 86.9% It has overfit issue, but considering that the dataset is large and representative and that the test scores are high, the model should be able to generalize reasonably well. 

In addition, I used PCA and truncated SVD for dimension reduction in an attempt to reduce model execution time. Both PCA and truncated SVD can capture around 94% of the variance with the first 20 components. When put into the logistic regression, the 2 algorithms reduced the fit time to 1/3 without significantly degrading the model's performance.

Please refer to the `Project.ipynb` file for details of the data and models 
