# Neural_Network_Charity_Analysis
Module 19

## Overview
Using what was learned in the module on machine learning and neural networks, the task was to create a binary classifier to predict whether applicants will be successful if funded by Alphabet Soup.

## Results
##### Data Preprocessing
1. What variable(s) are considered the target(s) for your model? For this analysis, the targeted data was the column IS_SUCCESSFUL. The machine learning and neural networks are using the available data in comparison to this column as a way to learn and then predict success of an applicant.

2. What variable(s) are considered to be the features for your model? The EIN and Name columns are identifiers rather than features to use in prediction so those were removed early in the preprocessing.  The remaining data points of Application_Type, Affiliation, Classification, Use_case, Organization, Status, Income_Amt, Special_Considerations, and Ask_Amt were used as features. During optimization both Status and Special_Considerations were also dropped as features in an attempt to reach a better predictive model.

3. What variable(s) are neither targets nor features, and should be removed from the input data?
Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take to try and increase model performance?
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
