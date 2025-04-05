# Handwritten-Digit-Detection-using-Neural-Network

## About the dataset used (MNIST):

The MNIST database (Modified National Institute of Standards and Technology database) is a large collection of handwritten digits. It has a training set of 60,000 examples, and a test set of 10,000 examples. It is a subset of a larger NIST Special Database 3 (digits written by employees of the United States Census Bureau) and Special Database 1 (digits written by high school students) which contain monochrome images of handwritten digits. The digits have been size-normalized and centered in a fixed-size image. The original black and white (bilevel) images from NIST were size normalized to fit in a 20x20 pixel box while preserving their aspect ratio. The resulting images contain grey levels as a result of the anti-aliasing technique used by the normalization algorithm. the images were centered in a 28x28 image by computing the center of mass of the pixels, and translating the image so as to position this point at the center of the 28x28 field.

## Project Overview

This project demonstrates a complete pipeline for handwritten digit recognition using a neural network trained on the MNIST dataset. A simple feedforward model was built with TensorFlow and trained on the dataset. The trained model was then integrated into a user-friendly Tkinter GUI, allowing users to draw digits on a canvas and get real-time predictions. The drawn image is preprocessed (resized, inverted, normalized, and centered) before being fed to the model for prediction.
