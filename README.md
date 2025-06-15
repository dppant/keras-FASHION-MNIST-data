# Fashion-MNIST CNN Classifier

This project implements a Convolutional Neural Network (CNN) using Keras to classify grayscale clothing images from the Fashion-MNIST dataset. The model was built and trained as part of a graduate-level Machine Learning course to demonstrate image classification using deep learning.

## Objective

To develop a CNN architecture using Keras that can classify fashion items with high accuracy using the Fashion-MNIST dataset.

## Dataset

Fashion-MNIST is a dataset of 60,000 training and 10,000 test grayscale images of 28x28 pixels representing 10 categories of fashion items.

### Label Categories

0 - T-shirt/top  
1 - Trouser  
2 - Pullover  
3 - Dress  
4 - Coat  
5 - Sandal  
6 - Shirt  
7 - Sneaker  
8 - Bag  
9 - Ankle boot  

## Preprocessing

- Reshaped input data to include a channel dimension: (28, 28, 1)
- Scaled pixel values to the range [0, 1]
- Converted class labels to one-hot encoded vectors

## Model Architecture

- Convolutional Layer: 27 filters of size 3x3, ReLU activation
- MaxPooling Layer: pool size 2x2
- Dropout Layer: 50%
- Flatten Layer
- Dense Layer: 100 neurons, ReLU activation
- Dropout Layer: 50%
- Output Layer: 10 neurons, softmax activation

## Compilation

- Loss Function: Categorical Crossentropy
- Optimizer: Adam
- Evaluation Metric: Accuracy

## Results

- Achieved test accuracy: **92%**
- Test error: **0.23**

## Summary

This project demonstrates how to preprocess image data and build a convolutional neural network from scratch using Keras. It highlights the importance of dropout for regularization and the effectiveness of CNNs in image classification tasks.

