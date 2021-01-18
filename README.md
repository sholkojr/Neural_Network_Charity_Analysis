# Neural_Network_Charity_Analysis

## Objective
Purpose of this analysis is to build a model to predict suitability of potential clients to provide monetary support as part of a charity's mission.

## Results

### Data Preprocessing
The variable "IS_SUCCESSFUL" was used as the target variable for this analysis.  

The model features included:
- APPLICATION_TY
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION
- STATUS
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- ASK_AMT

Features that were dropped from the model included "EIN" and "NAME", as they did not add value to the model.

### Compiling, Training and Evaluation of the Model
Trial and error was systematically used between 60 and 180 nodes on four layers and extending out to eight layers (the last three layers only up to 90 nodes. Nodes were increased in increments of 30.  Activation combinations were trialled with ReLU, exponential ReLU, tanh and linear functions

The Construction of the best neural network within the above parameters consisted of 4 layers, the first two layers consisted of 120 nodes each with the third and fourth layers consisting of 60 nodes each.  The first three layers used ReLU activation function, and the fourth layer utilised a linear activation functions.

With this construction, the best accuracy achieved was .7258, not within the 0.75 target but an improvement on the initial accuracy of .7244.

## Summary

Overall results were not quite at the 75% accuracy desired.  Recommend using different machine learning algorithms to see if better accuracy could be achieved.  Random Forrests would be a recommendation in particular because of the tabular nature of the data. 
