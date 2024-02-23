# CSGO-Round-Prediction
This project uses snapshot of each rounds to predict the winner of the round. The snapshot is recorded every 20 seconds since the round start until the round is decided. Each record contains information such as previous rounds' winner, remaining time of the round, each teams' HP and equipment, etc.

In the project, I trained and tuned a logistic regression model, a random forest model, and a shadow neural network model and compared their performance. In addition, I used PCA and truncated SVD for dimension reduction in attempts to reduce model execution time without d.

Please refer to the `Project.ipynb` file for details of the data and models 
