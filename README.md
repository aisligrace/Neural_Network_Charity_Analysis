# Neural_Network_Charity_Analysis
Module 19
## Overview
The overview for this project was to use machine learning and neural networks to create a binary classifier that is capable of predicting successful applicants funded by Alphabet Soup. We used Python and Jupyter notebook and many different libraries. 

## Results
Data Preprocessing
We cleaned our data by dropping the EIN and NAME column. The 'IS_SUCCESSFUL' column is our target. Our features are the columns 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANZIATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', and 'ASK_AMT'
We split the data into training and testing and scaled it.

Compiling, Training, and Evaluating the Model
We used two hidden layers, one with 30 and one with 80 neurons. We have one output layer as a binary classification. We used the activation function ReLU on the hidden layers and Sigmoid on the output layer, and Adam as the optimizer and binary_crossentropy as the loss activation.

The accuracy of our model started at 67%, and was 64.9% on our second try and 61% on our third. To try and improve the accuracy of our model, we increased the neurons on our hiddden layer, then we tried using three hidden layers. We also organized the 'ASK_AMT' column into buckets and organized the values by intervals. The last thing we did was switch the activation method from relu to tanh on the hidden layers. None of our additonal steps improved the accuracy of the model.

## Summary
We were unable to reach our goal of 75% accuracy, even with the three modifications we made. I would not recommend using this model. To improve, you could combine multiple decision model trees into a Random Forest Classifier using supervised machien learning. 
