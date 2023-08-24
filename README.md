# deep-learning-challenge
UCB Data Analysis Bootcamp Module 21 Deep Learning Challenge

## Installation

Google Colab is used to complete this challenge.


## Overview

This is the Module 21 challenge for the UC Berkeley Data Analyticd Boot Camp. In this challenge, the non-profit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. We are building a machine learning model that will use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

The Alphabet Soup's business team provided a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organizations, including:
  * EIN and NAME -- identification columns
  * APPLICATION_TYPE -- Alphabet Soup application type
  * AFFILIATION -- Affiliated sector of inductry
  * CLASSIFICATION -- Government organization classification
  * USE_CASE -- Use case for funding
  * ORGANIZATION -- Organization type
  * STATUS -- Active Status
  * INCOME_AMT -- Income classification
  * SPECIAL_CONSIDERATIONS -- Special considerations for application
  * ASK_AMT -- Funding amont requested
  * IS_SUCCESSFUL -- Was the money used effectively

## Results
### Data Processing
* The target variable is the IS_SUCCESSFUL column.
* Feature variables are the APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATION and ASK_AMT.
* Variables removed are the identification columns, that are EIN and NAME.

### Compiling, Training and Evaluating the Model
* Trained the model originally with 2 hidden layers, first layer with 80 neurons and second layer with 30 neurons, both layers have ReLU as the activation function. However, the model was unable to achieve the desired performance, so more neurons and/or hidden layers are added.
* The desired performance is an accuracy rate of 75% and higher, but unfortunately this model only reached 72.79% as its highest performance.
* Different methods are used in attempt to increase model performance:
  1. Increase the number of neurons
  2. Increase the number of hidden layers
  3. Use a different activation function
  4. All of item 1 to 3
  5. All of item 1 to 3, plus reducing the number of epoch

## Summary
While the attempts to optimize the model did not achieve the desired 75% accuracy rate, but it indeed increased the accuracy rate.

### Initial Model
![Original](https://github.com/sumiemma/deep-learning-challenge/assets/126445425/e3b52654-48df-4d48-b7f3-f7cb2f556eef)

### First Optimization Attempt
![First Attempt](https://github.com/sumiemma/deep-learning-challenge/assets/126445425/9f1340f1-a23d-4390-bb07-78315157fdae)

### Second Optimization Attempt
![Second Attempt](https://github.com/sumiemma/deep-learning-challenge/assets/126445425/a7761868-d876-41b4-829e-48e1c83e7c2f)

### Third Optimization Attempt
![Third Attempt](https://github.com/sumiemma/deep-learning-challenge/assets/126445425/a6ee058e-6615-4b68-9062-a8a9db00b983)

### Fourth Optimization Attempt
![Fourth Attempt](https://github.com/sumiemma/deep-learning-challenge/assets/126445425/3f80dd01-00d4-48e1-addc-0adf0c1dc4f7)

### Final Optimization Attempt
![Final Attempt](https://github.com/sumiemma/deep-learning-challenge/assets/126445425/9edfa052-d783-47da-ac23-6d6b35a4386e)

From the screenshots shown above, we can see the accuracy rate increased from 72.44% of the initial model, to the 72.79% of the fifth optimization attempt.

Some future optimization methods are to increase the amount of data, or to increase the feature variables of the existing data.
