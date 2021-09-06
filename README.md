# Neural_Network_Charity_Analysis

## Overview of the analysis
The purpose of this project is to analyze and classify the success of charitable donations using deep learning neural networks with the TensorFlow platform in Python. This project compromised of the following 3 steps:

    o  Preprocessing the data for the neural network
    o  Compile, Train and Evaluate the Model
    o  Optimizing the model


## Results

## Data Processing

    o  The columns EIN and NAME have been removed from the input data as they are identifying information.
    o  The column IS_SUCCESSFUL contains binary data referring to whether or not the charity donation was used effectively - This variable is then considered as the target for the deep learning neural network.
    o  The columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are the features of the model.
    o  Splitting into training and testing datasets and standardization have been applied to the features.


 

## Compiling Training and Evaluating the Model

    	o For my neural network model I had 2 hidden layers. My first layer had 80 neurons, the second has 30 there is also an output layer. 
	  The first and second hidden layer have the "relu" activation function and the activation function for the output layer is "sigmoid."

	o Were you able to achieve the target model performance?
 	  The model was not able to reach the target 75%. The accuracy for my model was 72%.
	  ![perfomance_model_1](https://github.com/amburu4159/Neural_Network_Charity_Analysis/blob/main/images/model_perfomance_1.PNG)

	o Steps taken to try and increase model performance
	 I applied bucketing to the feature ASK_AMT and organized the different values by intervals.
	 Then increased the number of neurons on one of the hidden layers, then we used a model with three hidden layers.
	 Also tried a different activation function (tanh) but none of these steps seemed to help improve the performance of the model


## Summary 

The deep learning neural network model did not reach the target of 75% accuracy. Regardless of the optimization added to the model, it could not getter an accuracy score better than 72%. The set target should be achievable using a deep learning model, so we can conclude that our model is not outperforming.
For better results, we could have used a supervised machine learning model such as the Random Forest Classifier to combine a multitude of decision trees to generate a classified output and evaluate its performance against our deep learning model.
