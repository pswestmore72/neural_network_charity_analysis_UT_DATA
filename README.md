# neural_network_charity_analysis_UT_DATA

## Purpose Overview

Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.

* Deliverable 1: Preprocessing Data for a Neural Network Model
* Deliverable 2: Compile, Train, and Evaluate the Model
* Deliverable 3: Optimize the Model
* Deliverable 4: A Written Report on the Neural Network Model (README.md)

## Results

### Data Preprocessing
- What variable(s) are considered the target(s) for your model?
  - **IS_SUCCESSFUL**
- What variable(s) are considered to be the features for your model?
  - **APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS**
- What variable(s) are neither targets nor features, and should be removed from the input data?
  - **EIN, NAME, ASK_AMT**

### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - First layer uses "relu", has 20 neurons
  - First layer uses "relu", has 10 neurons
  - First layer uses "tanh", has 10 neurons
  - This was done to attempt to optimize the shape of the model and the number of parameters for each layer, without over fitting the model 
- Were you able to achieve the target model performance?
  - No, achieved no noticable gain or loss in model performance
- What steps did you take to try and increase model performance?
  - Dropped the 'ASK_AMT' series
  - Binned the AFFILIATION and INC_AMT series
  - Added another hidden layer to the model with a different activation function (tanh)
  - Lowered the number of epochs needed to train model to 50

## Summary
 - Overall this models performs poorly,  