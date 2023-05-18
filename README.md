# Predicting-Scratch-Dies-on-Wafer-using-UNet
This repository contains my implementation of a UNet-based model for predicting whether a given die on a wafer map belongs to a scratch or not. The model is trained using labeled data that includes information about individual dies from multiple wafers.
Key Features:

Loads and preprocesses the wafer data from a provided zip file.
Provides an exploratory data analysis of the dataset, including the number of unique wafers and absent values.
Generates scratch banks for wafer images by grouping and analyzing the scratch dies.
Prepares test wafer images by converting die information into image arrays.
Implements a UNet-based model for scratch prediction, using a simple UNet architecture with convolutional and pooling layers.
Trains the model using the prepared dataset and evaluates it using dice loss and dice coefficient metrics.
Facilitates the prediction of scratch dies on test wafer images.
