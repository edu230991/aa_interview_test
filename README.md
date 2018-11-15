# Coding Excercise

## Introduction

The following excercise will try to quickly assess your timeseries modelling and data science skills.
You are provided with two pickle files, *train.pkl* and *test.pkl*. The names should be pretty self-explanatory.

*train.pkl* is a time-indexed pandas dataframe with two columns, "temperature" and "load". Units are degrees C and kWh respectively. Column "load" is a timeseries representing consumption of gas in a specific location in UK. Column "temperature" contains temperature measurements for the same location. *test.pkl* only contains the temperature column.

## Task

Your goal is to create an installable python package to forecast the load as a function of the datetime and temperature. 
The package should contain a class called *Model* with an sklearn-style API (at least *fit*, *predict* and *score* methods).

There are no limitations in terms of modelling techniques or extra data you might want to include. 
You are welcome to use part of the training set to tune your model.
If the training of the model takes more than 20 minutes on a normal laptop please make sure to include a method in the class to quickly load the trained model (e.g. by pickling it and adding it to the package).

You will be evaluated both on the score of the model on the test set as well as on the quality of the code. 


##  Delivering

You are welcome to reply to the email you will get from Orsted HR with a link to a GitHub or GitLab repo containing your code. Please include any dependencies in the *requirements.txt* file of your package. Please do not push to this repository, unless you want the other candidates to be able to look at your code!
The whole excercise should not take you a lot more than two to three hours. 
