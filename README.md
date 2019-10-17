# Machine Learning Homework - Exoplanet Exploration

![exoplanets.jpg](Images/exoplanets.jpg)

## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, different machine learning models are created that are capable of classifying candidate exoplanets from the raw dataset.

Following tasks are performed.

1. [Preprocess the raw data](#Preprocessing)
2. [Tune the models](#Tune-Model-Parameters)
3. [Compare two or more models](#Evaluate-Model-Performance)

- - -

### Preprocess the Data

* Check for NaN values and process them. 
* Performed Exploratory Data Analysis.
* Performed feature selection and removed unnecessary features.
* Performed label Encoding to convert Target label into numeric values.
* Used `MinMaxScaler` to scale the numerical data.
* Separated the data into training and testing data.

### Tune Model Parameters

* Used `GridSearch` to tune model parameters.
* Tuned and compared following models.
   1) [Logistic Regression model](logistic_regression_model.ipynb)
   2) [Decision Tree and Random Forest model](random_forrest_model.ipynb)
   3) [Support Vector Machine model](SVM_model.ipynb)
   4) [Deep Learning Model](deep_learning_model.ipynb)

### Reporting

* Train and Test Data Split:

 Data was split with 7:3 ratio for traina nd test data for all models.

* Logistic Regression Model:

This model gave an f-score of 0.81 for test data. After hypertuning of parameters, score remained at 0.81 only.

* Support Vector Machine Model:

This model gave a f-score of 0.75 on test data and after hyperparameter tuning, score improved to 0.78.

* Deep Learning Model

In this model, tried with both and 1 and 2 hidden layers and best score was obtained with 1 hidden layer.
Loss: 0.3501424750871673, Accuracy: 0.8603500723838806

* Decision Tree and random Forest Model

This model provided the best score and accuracy of all the models. 

Create a README that reports a comparison of each model's performance as well as a summary about your findings and any assumptions you can make based on your model (is your model good enough to predict new exoplanets? Why or why not? What would make your model be better at predicting new exoplanets?).

- - -

## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

* [Scikit-Learn Tutorial Part 1](https://www.youtube.com/watch?v=4PXAztQtoTg)

* [Scikit-Learn Tutorial Part 2](https://www.youtube.com/watch?v=gK43gtGh49o&t=5858s)

* [Grid Search](https://scikit-learn.org/stable/modules/grid_search.html)

- - -


##### © 2019 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
