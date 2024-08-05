# deep-learning-challenge
Repo for Module 21 Challenge

# Alphabet Soup Charity Funding Predictor
## Overview of the Analysis
The purpose of this analysis is to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup. Using a dataset containing metadata about organizations that have received funding from Alphabet Soup, we aim to build and optimize a neural network model to achieve a target predictive accuracy higher than 75%.

## Results
### Data Preprocessing
#### Target Variable:
    IS_SUCCESSFUL
#### Feature Variables:
    APPLICATION_TYPE
    AFFILIATION
    CLASSIFICATION
    USE_CASE
    ORGANIZATION
    STATUS
    INCOME_AMT
    SPECIAL_CONSIDERATIONS
    ASK_AMT
#### Removed Variables:
    EIN
    NAME
### Compiling, Training, and Evaluating the Model
#### Original Model:
####    Neurons and Layers:
            First hidden layer: 80 neurons, relu activation
            Second hidden layer: 30 neurons, relu activation
            Output layer: 1 neuron, sigmoid activation
            Epochs: 100
        Performance:
            Accuracy: 0.7281
            Loss: 0.5658
#### First Optimization:
####    Neurons and Layers:
            First hidden layer: 100 neurons, relu activation
            Second hidden layer: 50 neurons, relu activation
            Third hidden layer: 25 neurons, relu activation
            Output layer: 1 neuron, sigmoid activation
            Epochs: 200
        Performance:
            Accuracy: 0.7281
            Loss: 0.5658
#### Second Optimization:
####    Neurons and Layers:
            First hidden layer: 100 neurons, Relu activation
            Second hidden layer: 50 neurons, Relu activation
            Third hidden layer: 25 neurons, Relu activation
            Output layer: 1 neuron, sigmoid activation
            Epochs: 100
        Performance:
            Accuracy: 0.7268
            Loss: 0.6360
#### Third Optimization:
####    Neurons and Layers:
            First hidden layer: 100 neurons, LeakyReLU activation
            Second hidden layer: 50 neurons, LeakyReLU activation
            Third hidden layer: 25 neurons, LeakyReLU activation
            Output layer: 1 neuron, sigmoid activation
            Epochs: 200
        Performance:
            Accuracy: 0.7257
            Loss: 0.6301
## Summary
The deep learning model created for Alphabet Soup achieved an initial accuracy of 72.81%. Despite multiple optimization attempts, the target performance of 75% accuracy was not achieved. The optimizations included adding more neurons, adding an additional hidden layer, and experimenting with different activation functions.
