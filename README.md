# Module_19-Neural_Network_Charity_Analysis

# Overview

The purpose of this analysis was to harness an understanding of machine learning and neural networks to create a binary classification capable of predicting whether applicants would be successful of funded by our hypothetical firm: Alphabet Soup. Using a CSV contianing over 34,000 organizations which have recieved funding, we have preprocessed the data to be used in a Neural Network Model, compiled, trained, evaluated and optimized the model.

# Results

## Data Preprocessing

- The target for our model is the variable "IS_SUCCESSFUL", as the value in this column determines whether or not a venture was successful in a binary form.
- The features of our model are the variables "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_COUNSIDERATIONS", "ASK_AMT", and in the attept to improve the model, "NAME".
- "EIN" is neither a target nor a feature, and in the pre-optimization of the model "NAME" also fit this criteria and was deleted from the dataset.

## Compiling, Training, and Evaluating the Model

- Initially, the model contained 2 hidden layers, both of which with a relu activation function, and 80 and 30 neurons respectfully. In the optimized model, a third hidden layer was added and the second and third layers used a sigmoid activation function. These 3 layers had 100, 30, and 10 neurons respectfully.
- Yes, the optimized model had an accuracy score of .7897 as opposed to the inintial score of .7254.
- The first step I took was including "NAME" as a feature, which despite seeming arbitrary like the EIN, actually improved the model as organizations that appeaered often were more likely to be trustworthy and likely to succeed. Secondly, I added another hidden layer, changed the distribution of neurons, and changed the activation functions of the second and third hidden layers.

## Summarize

Overall, the improved model functioned fairly well, with a loss of .4462 and an accuracy score of .7897. A random forest of logistical regression model may be able to solve this problem, as they also deal with classification.
