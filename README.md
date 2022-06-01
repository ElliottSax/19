# Neural Network Charity Analysis
## Overview
Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.

With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization.
## Results
* Data Preprocessing
  - The variables that are considered to be targets for the model are the 'IS_SUCCESSFUL' column.
  - The variables that are considered to be feature columns are 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT', and 'SPECIAL_CONSIDERATIONS'.
  - The variables that are neither targets no features and were removed fromthe input data are 'STATUS', 'ASK_AMOUNT', 'NAME', AND 'EIN.'

* Compiling, Training, and Evaluating the Model
  -  For the initial model, there were wto layers with 8 neurons for layer one and 5 for layer two. It used the relu activation functions for the inputs and sigmoid for the output.  This model produced 66% accuracy.
  -  Trying to increase model performance:
    - Attempt 1: Three layers with 10 nodes for layer one, 7 for layer two, and four for layer 3. It also used relu and sigmoid for input and output respectively.  This model produced 53% accuracy.
    - Attempt 2: Two layers, 10 neurons for layer one and 7 for layer two, using relu and sigmoid for input and output.  This model produced 42% accuracy.
    - Attempt 3:  One layer with 10 neurons.  It changed the input function to tanh and output remained the same.  This model produced 52% accuracy.

## Summary
We did not reach the goal of 75% accuracy. Despite using a variety of number of number of layers and neurons, it did not increase more than the first attempt. I am inclined to think the issue is with not enough data, rather than the model.
