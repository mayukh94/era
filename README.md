<!-- markdownlint-disable MD030 -->

# ERA Session 5 Assignment - Mayukh

<a href="https://theschoolof.ai/#programs">Learn about the program here</a>

## 📝 Overview

### Building a Deep Neural Network for MNIST Dataset Classification

This repository contains an implementation of a deep neural network algorithm for accurately classifying the MNIST dataset. The algorithm utilizes convolutional neural networks (CNNs), max pooling, and the rectified linear unit (ReLU) activation function.

The main goal of this codebase is to develop a robust system that achieves high accuracy in classifying handwritten digits from the MNIST dataset. By leveraging CNNs, which are highly effective in image recognition tasks, along with max pooling and ReLU activation, the algorithm aims to achieve superior performance in digit recognition.

### File Descriptions

-   `model.py`

    The model.py file contains the implementation of the deep neural network model used for the MNIST dataset classification. It defines the architecture of the model, including the CNN layers, max pooling, and the ReLU activation function.
    
    The file defines a class `Net` which subclasses `nn.Module`.
    
    The `init` method defines the different layers involved in the neural network (CNN, FC etc.). 
    
    The `forward` method represents the forward pass of a neural network model. It performs a series of operations to transform and process the data. These operations include convolution, activation functions (ReLU), and max pooling. Finally the data is flattened and passed through fully connected layers. 
    
-   `utils.py`

    The file contains various utility functions that are used throughout the project. The functions include helper functions to 
    
    1. Check if cuda is available
    2. Plot loss and accuracy of the model
    3. Train a given model taking into account the device, model, criterion, data loader etc.
    4. Test a given model taking into account similar parameters as above.


-   `S5.ipynb`    
    
    The file serves as the entry point of the project. It orchestrates the execution of the entire system and manages the overall workflow. It imports and utilizes functions from model.py and utils.py to perform various tasks.
    
    It performs the following tasks
    
    1. Defines the transformations to be performed on the dataset for both training and testing purposes.
    2. Imports the required dataset and applies the requisite transforms
    3. Defines the batch size and readies the train and test data loaders.
    4. Instantiates the model defined in model.py and trains+tests the model (by utilising the train/test functions defined in the utility file) for 20 epochs while ensuring proper backpropagation.
    5. Finally it uses the plotting function defined in the utility file to plot the loss and accuracy of the model.

## ✨ Summary

Here's a generated summary of the model for an input of `(1, 28, 28)`

![Summary](/summary.png)

## 🙋 Support

Feel free to raise problems and solve them yourselves.

## 🙌 Contributing

No Contributions are allowed unfortunately :(
