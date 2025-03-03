# deep-learning-challenge


Overview of the analysis: Explain the purpose of this analysis.
The purpose of this analysis is to build and optimize a machine learning model that can make predictions based on input data. This involves several steps, including data preprocessing, feature selection, model training, and evaluation. The goal is to prepare the data, train the model, and evaluate its performance in order to make accurate predictions on if money was used successfully.

Results: Using bulleted lists and images to support your answers, address the following questions:
Data Preprocessing
What variable(s) are the target(s) for your model?
Target Variable: IS_SUCCESSFUL (whether the application was successful or not).

What variable(s) are the features for your model?
Feature Variables: All the other variables, including:
APPLICATION_TYPE_T10, APPLICATION_TYPE_T19, APPLICATION_TYPE_T3, etc.
CLASSIFICATION_C1200, CLASSIFICATION_C2000, etc.
AFFILIATION_Family/Parent, AFFILIATION_Independent, etc.
INCOME_AMT_1-9999, INCOME_AMT_10000-24999, etc.
Other variables related to different categories or organizations.

What variable(s) should be removed from the input data because they are neither targets nor features?
Variables that are irrelevant or do not contain information useful for predictions should be removed from the data.
Removed Variables:
EIN: This is an identifier that does not have any predictive value.
NAME: Similar to EIN, it is an identifier with no predictive value.
Any other variables with too many missing values or low variance may also be removed after careful evaluation.

Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
First Hidden Layer: 128 neurons — this number is chosen to capture enough complexity in the data, providing a good balance between model capacity and computational efficiency.
Second Hidden Layer: 64 neurons — reducing the number of neurons to avoid overfitting while still allowing the model to learn important patterns.
Output Layer: 1 neuron — since this is a binary classification task, we use a single output neuron to predict success or failure (using a sigmoid activation function).

Were you able to achieve the target model performance? 
No, I tried 4 differnet variable combinations and couldn't get the model performacne accuracy over 60%.'

What steps did you take in your attempts to increase model performance?
First, I removed application type, and status. That left the model performance accuracy at 55%.
Second, I removed application type, affiliation, use case, and status. That left the model performance accuracy at 53%.
Third, I removed everything but application type and classification. That left the model performance accuracy at 53%, as well.


Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.


