# Robotic_Inverse_Kinematics-using-Neural-Networks
## Overview
This project aims to implement a neural network-based solution for calculating the inverse kinematics of a 6-degree-of-freedom (6-DOF) robot. The inverse kinematics problem involves determining the joint angles necessary to achieve a desired end-effector position and orientation. Three types of neural network architectures are explored: feedforward neural networks and recurrent neural networks (RNNs) and Long Short-Term Memory (LSTM) architecture.

## Dataset
The dataset consists of samples of robot configurations and their corresponding end-effector positions in XYZ coordinates. Each sample contains:

### Input: 
XYZ position of the robot's end-effector.
### Output: 
Joint angles of 6-DOF Robot Manipulator required to reach the xyz position
# Models Implemented
## Feedforward Neural Network (FNN): 
A standard neural network architecture consisting of densely connected layers. This model maps the input XYZ positions to the output joint angles directly.

## Recurrent Neural Network (RNN) and LSTM: 
An RNN architecture and LSTM cells is used to capture sequential dependencies in the data, which may be present due to the nature of the robot's movements. The model takes sequences of XYZ positions as input and predicts the corresponding sequences of joint angles as output.

# Implementation
Python script implementing the LSTM model, feedforward neural network model and the RNN model using TensorFlow/Keras.
# Usage
Data Preparation: Prepare your dataset in CSV or other compatible formats. Ensure that each sample includes the input and the output.

# Training:

Run feedforward_nn.py to train the feedforward neural network model.
Run rnn_lstm.py to train the RNN with LSTM model.
Adjust hyperparameters, network architecture, and training settings as needed.
Evaluation: Evaluate the trained models using appropriate metrics to assess their performance. This may include loss functions, accuracy, or other domain-specific metrics.

# Inference: 
Use the trained models to predict the end-effector positions for new robot configurations.
