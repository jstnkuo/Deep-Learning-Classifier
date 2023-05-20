## Overview of the analysis:
The purpose of this analysis is to build a machine learning model that predicts whether applicants to the charity organization Alphabet Soup will be successful in receiving funding. <br>
The analysis involves preprocessing and transforming the input data, training a deep neural network model, evaluating, and optimizing its performance.

## Results: 
**Data Prepcrocessing**: <br>
• The target for this model is the 'IS_SUCCESSFUL' column <br>
• The features include all columns in the dataset excluding the target column, 'NAME', 'EIN', and 'STATUS' <br>
• 'NAME' and 'EIN' are neither targets nor features so they were removed from input data <br>
<br>
**Compiling, Training, and Evaluating the Model** <br>
• In the original model, two layers were chosen with 80 and 30 neurons, respectively. 'Relu' was selected as the activation function. <br>
• In the optimized model, an additional layer was added. 20 neurons were selected for the first layer as the result of dividing the number of columns by 2, 10 neurons for the second, and 5 for the third . 'Relu' remained as the activation function <br>
