# Forecasting-Data


**Model Architecture.**
Here we have use 3 layers
1.Input Layer is used to take the data layer.
2.The input data needs to be shaped as [samples, time steps, features] for an LSTM model.
4.For a univariate time series, there would be a single feature - the value at each time step.
5.Multiple LSTM layers allow learning higher-level temporal abstractions and dependencies.


Common to have 2-3 LSTM layers with dropout between them.
Number of memory units in LSTM layers is a key hyperparameter governing model capacity.
The output shape should match the prediction target. For univariate forecasting this is usually a single unit.
Can activate with a linear activation since it's regression. Other options could be softmax for classification.
**Results**
RNN model performed better than the MLP model as we can see from the results. the lower the loss value the better the function.
MLP Model - MAE: 0.07494115616399873
MLP Model - RMSE: 0.09463825455749447
RNN Model - MAE: 0.06910899406415853
RNN Model - RMSE: 0.08700322850940238
