# Predict-Accident-Severity

## Objective

The aim of the project is to predict the severity of an accident due to various features like road conditions, geographic location, weather conditions and type of vehicles. The prediction is achieved using three models- Naive Bayes, Suport Vector Machine and Neural Network and the three models are compared based on the accuracy score.

## Methodology

* Common data cleaning, data analysis and data transformation techniques were applied. 

* In Naive Bayes- based on the data type, Gaussian NB, Categorical NB and multinomial NB was performed and the results were combined. 

* The neural network classification model was built using different combinations of hyperparameters to find the best combination based on the validation accuracy. The tuning parameters used are:Number of hidden layers,Number of neurons,Activation function,Learning rate,Momentum,Dropout

* We experiemented with different types of SVC kernels- Linear, Poly, RBF and Poly SVC was chosen has it yielded the best results. 

## Experimentation 

Below are some methods we tried for one or more of the models, but it wasn't implemented since the accuracy score was low or it was computationally heavy:

Since the data is imbalanced, we tried NearMiss to undersample the data and SMOTE to oversample the data
We tried two dimension reduction techniques -PCA/MCA and Autoencoder, both of these methods were computationally heavy and didn't vary the scores by more than 1 percent.
Varying the threshold of the probability to determine the class for prediction.
For Neural Network, we didn't use feature selection because it was lowering down the model accuracy. The best accuracy received was by taking in all the features.

## Conclusion 

The final results on the test set for all the above three models are:
Naive Bayes - 75.40%
Neural Network - 74.33%
Support Vector Machine - 75.05%
