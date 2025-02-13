# deep-learning-challenge

## Overview
- The purpose of this project is to analyze the records of organizations which have received funding from Alphabe Soup in the past,
in order to predict which organizations will be successful in their ventures in the future.


### Data Preprocessing
What variable(s) are the target(s) for your model?
- Venture Success
What variable(s) are the features for your model?
- Application Type, Affiliation, Classification, Use Case, Organization, Status, Income Amount, Special Considerations, and Ask Amount
What variable(s) should be removed from the input data because they are neither targets nor features?
- Organization Name and EIN#

### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
- The final neural network contains three Dense layers, each followed by a BatchNormalization and Dropout layer, and one output layer
- They utilize ReLu and Sigmoid functions, because those are best suited to the type of binary classification task being attempted here
- The input layer has 40 nodes, matching the number of features being input. From there, the number of nodes decreases in each layer, concluding in a single node for the output layer

### Were you able to achieve the target model performance?
- Ultimately, no. I tried many iterations of this model, but it never breached 73% accuracy

### What steps did you take in your attempts to increase model performance?
- I added an additional Dense layer and ten more epochs, as well as BatchNormalization, Dropout layers, and callbacks to reduce the learning rate if the model plateaued. 

## Summary: 
This deep learning model analyzed the features of previous Alphabet Soup ventures, and managed to use them to predict the success of future ventures with 73% accuracy. Due to the fact that the overall model accuracy remained the same across several drastic iterations, if I were to try again to improve it, I would start with including k-fold validation to ensure that the issues were not due to the vagaries of a specifc train/test split.
