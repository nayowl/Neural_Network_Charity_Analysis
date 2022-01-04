# Neural_Network_Charity_Analysis
## 1. Overview
Alphabet Soup is a philanthropic foundation dedicated to helping organizations that protect the environment improve well-being and unify the world. By using machine learning and neural network, this project will use the features in the charity dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

The following tasks will be performed for the analysis:
* Preprocessing Data for a Neural Network Model
* Compile, Train, and Evaluate the Model
* Optimize the Model


## 2.Resources
Data Source: charity_data.csv

Software: Python, Jupyter Notebook

## 3. Results
### Data Preprocessing
#### What variable(s) are considered the target(s) for your model?
The target of the model is “IS_SUCCESSFULL” column.

#### What variable(s) are considered to be the features for your model?
All variables in the dataframe are considered to be the features of the model except "EIN" and "NAME" column

#### What variable(s) are neither targets nor features, and should be removed from the input data? 
"EIN" and "NAME" column are neither targets nor features and shoul be removed from the input data because it's meaningless or can cause confusion for the model 

### Compiling, Training, and Evaluating the Model
#### How many neurons, layers, and activation functions did you select for your neural network model, and why?
I used 3 layers , 
#### Were you able to achieve the target model performance?

#### What steps did you take to try and increase model performance? 

## 3. Summary
