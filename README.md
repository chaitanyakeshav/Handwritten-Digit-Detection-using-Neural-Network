# Handwritten-Digit-Detection-using-Neural-Network-and-Live-Drawing-Detection

## About the dataset used (MNIST):

The MNIST database (Modified National Institute of Standards and Technology database) is a large collection of handwritten digits. It has a training set of 60,000 examples, and a test set of 10,000 examples. It is a subset of a larger NIST Special Database 3 (digits written by employees of the United States Census Bureau) and Special Database 1 (digits written by high school students) which contain monochrome images of handwritten digits. The digits have been size-normalized and centered in a fixed-size image. The original black and white (bilevel) images from NIST were size normalized to fit in a 20x20 pixel box while preserving their aspect ratio. The resulting images contain grey levels as a result of the anti-aliasing technique used by the normalization algorithm. the images were centered in a 28x28 image by computing the center of mass of the pixels, and translating the image so as to position this point at the center of the 28x28 field.

## Project Overview

This project demonstrates a complete pipeline for handwritten digit recognition using a neural network trained on the MNIST dataset. A simple feedforward model was built with TensorFlow and trained on the dataset. The trained model was then integrated into a user-friendly Tkinter GUI, allowing users to draw digits on a canvas and get real-time predictions. The drawn image is preprocessed (resized, inverted, normalized, and centered) before being fed to the model for prediction.

## Neural Network Architecture

This project employs a simple Neural Network using TensorFlow. The network begins with an input layer of 784 nodes, corresponding to the flattened 28x28 grayscale pixel values of the MNIST digit images. It is followed by two hidden layers — the first with 128 neurons and the second with 64 neurons — both using the ReLU activation function to introduce non-linearity. The output layer contains 10 neurons with a softmax activation, providing a probability distribution over the digit classes (0 through 9). The model is compiled using Stochastic Gradient Descent (SGD) and trained with categorical crossentropy, a standard loss function for multi-class classification tasks.

## Live Drawn Digit Detection : Tkinter GUI Integration

At last I have used simple yet effective Tkinter-based graphical user interface that allows users to draw digits directly on a canvas. Once a digit is drawn, the image is preprocessed — resized to 28x28 pixels, colors inverted, normalized, thresholded to remove noise, and centered using the digit's center of mass. The processed image is then passed to the trained neural network model, which predicts the digit in real time. The predicted digit is displayed in the GUI, making the model's functionality easily testable and interactive for users.
