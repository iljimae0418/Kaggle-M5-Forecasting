# Kaggle M5 Forecasting Contest 
[Competition Link](https://www.kaggle.com/c/m5-forecasting-accuracy/overview)

- M5 LSTM base 1.ipynb : splitting such that x_train contains a seven day timestep (d_i to d_{i+6}) and y_train contains a seven day timestep (d_{i+1} to d_{i+7}). Uses a one layer LSTM. Scores 3.07 on the public leaderboard. 

- M5 LSTM base 2.ipynb : splitting such that x_train contains a seven day window (d_i to d_{i+6}) and y_train contains a one day timestep (d_{i+7}). Uses a one layer LSTM. Scores 3.00 on the public leaderboard.  

- m5_one_timestep_kth.ipynb: splitting such that x_train contains a seven day window (d_i to d_{i+6}) and y_train contains a one day timestep (d_{i+7}). LSTM returns output shape (None, 128). Picks every kth datapoint for training for predicting t+k. Scores 1.01 on the public leaderboard.  

- m5_one_timestep_append.ipynb: same as m5_one_timestep_kth.ipynb but re-uses predicted value for next prediction (instead of picking kth). So when predicting t+k, uses t+1,...,t+k-1 that were predicted using the model. Scores 1.43 on the leaderboard.  

- m5_kth_standardized.ipynb: same as m5_one_timestep_kth.ipynb but standardizes the data row-wise. Scores 1.59 on the leaderboard. 
