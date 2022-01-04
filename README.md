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
#### :question: What variable(s) are considered the target(s) for your model?
The target of the model is “IS_SUCCESSFULL” column.

#### :question: What variable(s) are considered to be the features for your model?
All variables in the dataframe are considered to be the features of the model except "EIN" and "NAME" column

#### :question: What variable(s) are neither targets nor features, and should be removed from the input data? 
"EIN" and "NAME" column are neither targets nor features and shoul be removed from the input data because it's meaningless or can cause confusion for the model 

### Compiling, Training, and Evaluating the Model
#### :question: How many neurons, layers, and activation functions did you select for your neural network model, and why?
* I used 3 layers , with 130 nodes in layer 1, 60 nodes in layer 2, and 25 nodes in layer 3. The first layer has almost double amount of the input layer as the recommendation. 
* All of three layer using relu activation, and for the ouput layer using sigmoid. This because the activation has the best accuracy for this model
* The epoch is 200, because the model has more improvement on 200 epoch compared to 100 epoch.
<p align="center">
    <img src="https://user-images.githubusercontent.com/88597187/148017066-eba6602e-b512-4692-99a8-e2f5008ced23.png"  width="600" height="300"/>
        
</p>

<p align="center">
  <sub>Figure 1 Model Evaluation </sub>
</p>

#### :question: Were you able to achieve the target model performance?
Yes, i am able to achieve 75.359% , compared to 72.37% before the optimization
<p align="center">
    <img src="https://user-images.githubusercontent.com/88597187/148018364-039a3327-3d40-43ca-b17f-eb517f2ac63d.png"  width="600" height="100"/>
        
</p>

<p align="center">
  <sub>Figure 2 Accuracy of Model after Optimization</sub>
</p>

#### :question: What steps did you take to try and increase model performance? 

To increase the model performance , the steps are :

* Add "NAME"column to add more features to data. Replace "NAME" value  into "other" bin if the count <100 and retain the rest. 
* Change the condition of appilcation_type_counts when binning the data from <500 to <700
* Binned ASK_AMT value to 2 bin 5000 and >5000
* Add 1 hidden layer and increase the neuron on each layer from (80,30 ) to (130,60,25)
* Change epoch to 200 instead of 100

## 3. Summary
The model  after optimization has 0.5679943561553955 loss and Accuracy  0.7535859942436218. This means that he probability model to fail is 56.7994% and  the probability model to be accurate is 75.359% .

#### Suggestion 
 To Improve the accuracy of the model , we can add more features or add more data to the dataset. And to compare the performance we can try to use the random forest.The random forest has comparable accuracy to the deep learning model but it has less code and faster performance. 

