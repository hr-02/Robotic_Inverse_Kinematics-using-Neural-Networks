# Robotic_Inverse_Kinematics-using-Neural-Networks
6-DOF Robot Inverse Kinematics with Neural Networks
#Overview
Overview
This project aims to implement a neural network-based solution for calculating the inverse kinematics of a 6-degree-of-freedom (6-DOF) robot. The inverse kinematics problem involves determining the joint angles necessary to achieve a desired end-effector position and orientation. Two types of neural network architectures are explored: feedforward neural networks and recurrent neural networks (RNNs) with Long Short-Term Memory (LSTM) cells.

Dataset
The dataset consists of samples of robot configurations and their corresponding end-effector positions in XYZ coordinates. Each sample contains:

Input: Joint angles representing the configuration of the 6-DOF robot.
Output: XYZ position of the robot's end-effector corresponding to the given joint angles.
Models Implemented
Feedforward Neural Network (FNN): A standard neural network architecture consisting of densely connected layers. This model maps the input joint angles to the output XYZ positions directly.

Recurrent Neural Network (RNN) with LSTM: An RNN architecture with LSTM cells is used to capture sequential dependencies in the data, which may be present due to the nature of the robot's movements. The model takes sequences of joint angles as input and predicts the corresponding sequences of XYZ positions.

Implementation
feedforward_nn.py: Python script implementing the feedforward neural network model using TensorFlow/Keras.
rnn_lstm.py: Python script implementing the RNN with LSTM model using TensorFlow/Keras.
Usage
Data Preparation: Prepare your dataset in CSV or other compatible formats. Ensure that each sample includes the input joint angles and the corresponding output XYZ positions.

Training:

Run feedforward_nn.py to train the feedforward neural network model.
Run rnn_lstm.py to train the RNN with LSTM model.
Adjust hyperparameters, network architecture, and training settings as needed.
Evaluation: Evaluate the trained models using appropriate metrics to assess their performance. This may include loss functions, accuracy, or other domain-specific metrics.

Inference: Use the trained models to predict the end-effector positions for new robot configurations.
