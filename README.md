# Kaggle M5 Forecasting Contest 
[Competition Link](https://www.kaggle.com/c/m5-forecasting-accuracy/overview)

- M5 LSTM base 1 : splitting such that x_train contains a seven day timestep (d_i to d_{i+6}) and y_train contains a seven day timestep (d_{i+1} to d_{i+7}). Uses a one layer LSTM. 

- M5 LSTM base 2: splitting such that x_train contains a seven day window (d_i to d_{i+6}) and y_train contains a one day timestep (d_{i+7}). Uses a one layer LSTM. 
