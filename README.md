# Student Exam Marks Prediction

<img width="695" alt="Capture" src="https://user-images.githubusercontent.com/89142569/229309274-80d5d987-14c3-4840-8457-e31b2dc9e1fb.PNG">


This data science project walks through the end to end implementation of prediction of a student marks. The code structure almost replicates the modular architecture. At first, a machine learning model is built and the best model among the various algoetihms is choosen. A flask server is written that takes the model to serve http requests.A website is built using the html
that allows the user to enter the various parameters required to the predict the marks. Later the docker
container is built with the model and deployed to the heroku cloud. The entire process is done automatically by using GitHub actions.

## Data Set Information
* Dataset Source - https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977
* gender : sex of students -> (Male/female)
* race/ethnicity : ethnicity of students -> (Group A, B,C, D,E)
* parental level of education : parents' final education ->(bachelor's degree,some college,master's     degree,associate's degree,high school)
* lunch : having lunch before test (standard or free/reduced)
* test preparation course : complete or not complete before test
* math score
* reading score
* writing score

## Life cycle of ML Project

This project involves all the data science concepts like data collection, data checking, exploratory data analysis, data pre processing , model training, hyper parameter tuning, chossing the best model based on various metrics and saving the best model. Refere the notebook section for more information/code.

## Building Flask and Docker container

A website is built using the html that allows the user to enter the various parameters required to the predict the marks. Later the flask server uses the best model and serves the http request by predicting the maths marks of the student once all the required paramters are given by the user through the UI.

Own docker images is built through the Dockerfile and the app is deployed in the Heroku cloud through the GitHub action.

