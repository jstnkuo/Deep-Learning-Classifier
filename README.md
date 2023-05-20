## Overview of the analysis
The purpose of this analysis is to build a machine learning model that predicts whether applicants to the charity organization Alphabet Soup will be successful in receiving funding. <br>
The analysis involves preprocessing and transforming the input data, training a deep neural network model, evaluating, and optimizing its performance.

## Results
**Data Prepcrocessing** <br>
• The target for this model is the 'IS_SUCCESSFUL' column <br>
• The features include all columns in the dataset excluding the target column, 'NAME', 'EIN', and 'STATUS' <br>
• 'NAME' and 'EIN' are neither targets nor features so they were removed from input data <br>
<br>
**Compiling, Training, and Evaluating the Model** <br>
• In the original model, two layers were chosen with 80 and 30 neurons, respectively. 'Relu' was selected as the activation function. <br>
• In the optimized model, an additional layer was added. 20 neurons were selected for the first layer as the result of dividing the number of columns by 2. Following the idea of dividing by 2, 10 neurons for the second layer, and 5 for the third. 'Relu' remained as the activation function <br>
<br>
• The optimized model reached a 74% accuracy at its peak, which failed to hit the target accuray of 75%. <br>
![alt text](https://github.com/jstnkuo/Deep-Learning-Classifier/blob/main/images/optimized_accuracy.png) <br>
• My attempts to increase model performance included removing unncessary features, adding another hidden layer, increasing epochs, and changing numbers of neurons. <br>
## Summary
The overall results of this deep learning model was not up to par in hitting the target accuracy of 75%, although it was close. <br>
In a different attempt I would recommend using RandomForest to solve this classification problem for the following reasons: <br> 
1) Handling categorical features: Random Forest handles categorical features naturally without requiring one-hot encoding. This can be advantageous when working with categorical variables like 'APPLICATION_TYPE' and 'CLASSIFICATION' in the dataset. <br>
2) 
