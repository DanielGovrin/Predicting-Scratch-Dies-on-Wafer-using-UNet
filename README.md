# Description:

This repository contains the code and implementation of a scratch prediction model using the UNet architecture. The model is designed to accurately predict whether a given die on a wafer belongs to a scratch or not. It leverages wafer maps, including information such as the wafer name, die coordinates, and indicators of good or scratch dies.

# Key Features:

Utilizes the UNet architecture for effective image segmentation and scratch prediction.
Trained on a labeled dataset consisting of wafer maps and associated scratch annotations.
Provides a reliable prediction of whether a die belongs to a scratch or not.
Handles the identification of both good and scratch dies on the wafer.

# The code performs the following steps:

Loads the data from a zip file containing the wafer and test data.

Preprocesses the wafer data, including grouping by wafer name, checking for absent values, and visualizing scratch die counts.
Constructs a scratch bank dictionary to store scratch banks associated with each wafer size.
Preprocesses the test data, setting corresponding pixels to white for bad dies.
Splits the dataset into training and validation sets using a specified test size.
Implements the UNet model architecture using TensorFlow and Keras.
Compiles the model with the Adam optimizer and a custom dice loss function.
Trains the model on the training data for a specified number of epochs.
The scratch prediction model presented in this repository is applicable in the semiconductor industry, aiding in the early detection and prevention of manufacturing defects. By accurately identifying scratch dies, it contributes to improved yield and quality control.
