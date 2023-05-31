# Challenge21-deep-learning
Overview of the analysis: In this project a binary classification model has been created that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset.


Results:
target variable: y='IS_SUCCESSFUL';
feature variables: X=[
APPLICATION_TYPE,
AFFILIATION,
CLASSIFICATION,
USE_CASE,
ORGANIZATION,
STATUS,
INCOME_AMT,
SPECIAL_CONSIDERATIONS,
ASK_AMT]


In order to improve the model I tried to use different methods such as:
1. Remove/add binary variables: 'STATUS', 'SPECIAL_CONSIDERATIONS',
2. Remove outliers from numerical variable: 'ASK_AMT',
3. Change number of neurons and number of layers,
4. Change activation function on the first and second hidden layer: from 'relu' to 'sigmoid'
5. Choose a different algorithm such as Stochastic Gradient Descent (SGD).
Finally, I dropped 'SPECIAL_CONSIDERATIONS' variable along with 'EIN' and 'NAME',
used 64 and 64 hidden layers, and used SGD algorithm since that accuracy is better.


Summary: The model can predict whether the Alphabet Soup-funded organization is successful or not, but it should be improved. 
The customers who have 'Funding amount requested' ('ASK_AMT') as zero should be further divided into more specific subcategories.
'INCOME_AMT' is better to be numeric.
