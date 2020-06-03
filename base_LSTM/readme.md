# Kaggle M5 Forecasting Contest 
[Competition Link](https://www.kaggle.com/c/m5-forecasting-accuracy/overview)

- M5 LSTM base 1.ipynb : splitting such that x_train contains a seven day timestep (d_i to d_{i+6}) and y_train contains a seven day timestep (d_{i+1} to d_{i+7}). Uses a one layer LSTM. Scores 3.07 on the public leaderboard. 

- M5 LSTM base 2.ipynb : splitting such that x_train contains a seven day window (d_i to d_{i+6}) and y_train contains a one day timestep (d_{i+7}). Uses a one layer LSTM. Scores 3.00 on the public leaderboard.  

- m5_one_timestep_kth.ipynb: splitting such that x_train contains a seven day window (d_i to d_{i+6}) and y_train contains a one day timestep (d_{i+7}). LSTM returns output shape (None, 128). Scores 1.01 on the public leaderboard.  
