# Cars
This repository consists of 2 models. One is a Regression model which predicts the price of the car. The second model is a Classification model which classifies different models of a Vehicle.

# Price Predictor

This is a Regression problem 

The missing values were ‘?’ in the dataset, which I handled by using SimpleImputer and pandas. 

The 25 features in the dataset helped me to predict the prices of the cars 

The most important features in the dataset are: 
  Make or the company of the car
  Aspiration
  drive-wheels
  body-style
  engine-type
  num-of-cylinders
  horsepower
  peak-rpm 

Used Label Encoding for num-of-doors and num-of-cylinders features. 
Used One Hot Encoding for all the other categorical features. 

Split the test and train data with 20% data in test dataset. 

Fit different Regression models like Linear Regression, Decision Tree Regressor and Random Forest Regressor. 

The ‘final_model’ is the Random Forest Regressor which got 95% score which is the best when compared to other models. 

The result of the model is: 
Score  –>  95% 
Mean Squared Error -> 3945981 
Mean Absolute Error -> 1330

# Classifier
This is a Classification problem

Understanding the Dataset
  Imported the ‘car_class.csv’ dataset and converted to a Data Frame
	There were no missing values in the dataset

Pre-processing
	Plotted the co-relation of the dataset and dropped the most co-related features
	All the features have good importance in classification
	Handled the outliers by using 25th and 75th quartile range and replaced the values.

Building the Model
  Fit different models like K Nearest Neighbors, Decision Tree, Random Forest, SVC and Logistic Regression.
  Analysed the performance of each model by using metrics such as Accuracy and Classification matrix.
  Logistic Regression model performed the best

Final Model
Logistic Regression model is the final model with Accuracy of approximately 83%
The model predicted the 0 and 3 classes perfectly and majority of the 1, 2 classes were predicted correctly.
