## Time Series Prediction using Simple Recurrent Neural Network (RNN)

### Description

This script demonstrates how to use a Simple Recurrent Neural Network (RNN) to predict future values in a time series dataset. The dataset contains a single time series, and the goal is to predict the next value based on the previous values.

### Data Preprocessing

The script reads a time series dataset from a CSV file and preprocesses it by scaling the values using Min-Max scaling. It splits the dataset into training and testing sets and creates input-output pairs for training the RNN model.

### Model Architecture

The RNN model is defined using the Keras Sequential API. It consists of a single SimpleRNN layer followed by a Dense output layer. The input shape of the RNN layer is determined by the look-back parameter, which specifies the number of previous time steps to consider for prediction.

### Training

The model is trained using the training data with the mean squared error loss function and the Adam optimizer. The training process runs for a specified number of epochs with a batch size of 1.

### Prediction

After training, the model is used to predict future values in the time series dataset. Both training and testing predictions are generated and inverse scaled to obtain the actual predicted values.

### Visualization

The script visualizes the training and testing predictions along with the actual values to evaluate the model's performance in capturing the underlying patterns in the time series data.

