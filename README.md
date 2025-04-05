# Handwritten-Digit-Detection-using-Neural-Network

## About the dataset used (MNIST):

The MNIST database (Modified National Institute of Standards and Technology database) is a large collection of handwritten digits. It has a training set of 60,000 examples, and a test set of 10,000 examples. It is a subset of a larger NIST Special Database 3 (digits written by employees of the United States Census Bureau) and Special Database 1 (digits written by high school students) which contain monochrome images of handwritten digits. The digits have been size-normalized and centered in a fixed-size image. The original black and white (bilevel) images from NIST were size normalized to fit in a 20x20 pixel box while preserving their aspect ratio. The resulting images contain grey levels as a result of the anti-aliasing technique used by the normalization algorithm. the images were centered in a 28x28 image by computing the center of mass of the pixels, and translating the image so as to position this point at the center of the 28x28 field.

## Project Overview
This project showcases the complete pipeline of building a handwritten digit recognition system using deep learning and integrating it into a Tkinter-based graphical interface.

What I’ve Done:
Built a Neural Network

Used TensorFlow to build and train a simple feedforward neural network.

Trained the model on the complete MNIST dataset (no train-test split for this version) to recognize digits from 0 to 9.

Saved the trained model as mnist_model.h5.

Developed a Tkinter GUI Application

Created an interactive canvas where users can draw digits using the mouse.

Captured the drawing, resized and preprocessed it to match the format of MNIST images (28x28 grayscale, normalized, centered).

Used the trained model to predict the digit drawn by the user.

Displayed the prediction along with the processed image for better understanding.

Added Image Processing Enhancements

Implemented color inversion and normalization.

Applied centering using center of mass to improve prediction accuracy.

Visualized the processed input using Matplotlib for transparency.
