# Optimizing LSTM Models for Time Series Forecasting: A Meta-Heuristic Approach

This project employs a meta-heuristic optimization approach to fine-tune the architecture of a neural network for time series data analysis, specifically focusing on electronic device production data. The objective is to optimize the model's parameters to achieve the most accurate predictions in the test set sequence.

## Hyperparameters
The hyperparameters considered in this study include:
- `look_back`: The number of previous sequences used to predict the next step.
- `Nunits`: The number of nodes in hidden layers.
- `activation`: The type of activation function used in hidden layers.
- `NLayer`: The number of hidden layers.

## Model and Optimization Method
The LSTM (Long Short-Term Memory) model is utilized to forecast future sequences in the time series data, although alternative models could also be explored. The "GlobalBestPSO" method from the `pyswarms` library is employed to search the hyper-parameter space for optimal values that minimize the model's loss. The mean squared error method is used to quantify the loss in predicting future sequences.

## Model Evaluation
Following the determination of optimal hyper-parameter values, they are utilized to construct the optimal model. The performance of this model is evaluated by comparing its predictions with the actual values in the test set.
