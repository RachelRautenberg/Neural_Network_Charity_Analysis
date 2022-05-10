# Neural_Network_Charity_Analysis
Module 19

## Overview

Using what was learned in the module on machine learning and neural networks, the task was to create a binary classifier to predict whether applicants will be successful if funded by Alphabet Soup.

## Results

##### Data Preprocessing
1. What variable(s) are considered the target(s) for your model? For this analysis, the targeted data was the column IS_SUCCESSFUL. The machine learning and neural networks are using the available data in comparison to this column as a way to learn and then predict success of an applicant.

2. What variable(s) are considered to be the features for your model? The EIN and Name columns are identifiers rather than features to use in prediction so those were removed early in the preprocessing.  The remaining data points of Application_Type, Affiliation, Classification, Use_case, Organization, Status, Income_Amt, Special_Considerations, and Ask_Amt were used as features. During optimization both Status and Special_Considerations were also dropped as features in an attempt to reach a better predictive model.

3. What variable(s) are neither targets nor features, and should be removed from the input data? For the initial learning and neural network model the EIN and Name data points were neither target nor feature.  When working through optimization Status and Special_Considerations also become not a target nor feature. 

##### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
     
     | During the initial modeling, two layers were used with 92 and 40 neurons respective in the first and second later.  Two layers was chosen because we are not working with a very large dataset, but enough where more than a basic neural network is likely to produce good results.  The first layer of neurons, 92 was selected by following the rule of thumb approximation of 2x more than input features.  The second layer of 40 neurons was chosen as each layer should be less than the one before and more than the final output.  Similar process was used in optimization.  For the first layer, 128 neurons was used - which is roughly 3x the input features, that was halved to get 64 neurons for the second layer, then halved again to get 32 neurons for the third layer.  A fourth hidden layer was added, but then removed as it did not significantly change the accuracy.

Were you able to achieve the target model performance?

     |  Target of 75% accuracy was not acheived. (But I would love to know the answer to how it can be done!)
     
What steps did you take to try and increase model performance?

    | Five steps were taken in an attempt to optimize the model to 75% accuracy.  Each attempt except for the final was run as a stand-alone change, so previous changes were removed and the new change was run. First attempt, addition columns were dropped. Second attempt, increased neurons in the hidden layers.  Third attempt, increased the hidden laters. Fourth attempt, changed the activation function.  Fifth attempt, put all of the other four attempts together in on optimization run. 
    
## Summary

The initial and optimized models did not reach the target of 75% accuracy.  I suggest a few things for improving the model funcationality. First, I would start by, assuming a 'real world' environment, returning to where the data came from to ask or better understand each of the columns to determine if any of the other columns are not necessary for the predictive modeling. I would also run an importances analysis to see if there are features that have lower contribution which could lead to additional model adjustments.  Finally, at this stage in my machine learning journey, I would discuss with colleagues or other trusted data analysis network contacts to see if they had suggestions that I had not yet attempted. 
