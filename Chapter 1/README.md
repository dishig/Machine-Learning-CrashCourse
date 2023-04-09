# Chapter 1: Intro to Machine Learning


## Agenda:
1. Basics of Machine Learning
2. Basics of Regression 
3. Regression Assignment

## Basics of Machine Learning

[![Video: Machine Learning Basics | What Is Machine Learning? | Introduction To Machine Learning | Simplilearn](https://img.youtube.com/vi/ukzFI9rgwfU/0.jpg)](https://www.youtube.com/watch?v=ukzFI9rgwfU "Machine Learning Basics | What Is Machine Learning? | Introduction To Machine Learning | Simplilearn")

### Quiz 1
Try to Answer the 3 types of problem at timestamp [5:50](https://youtu.be/ukzFI9rgwfU?t=351) 

Link to Answer: [Answers](#solutions) 
> **Note:** Don't jump to the answers directly without trying to solve/google/ask on your own.

## Basics of Regression
Watch the below video to understand the Supervised Machine Learning Technique of Linear Regression.
[![Video: Regression Basics](https://img.youtube.com/vi/PaFPbb66DxQ/0.jpg)](https://www.youtube.com/watch?v=PaFPbb66DxQ "The Main Ideas of Fitting a Line to Data (The Main Ideas of Least Squares and Linear Regression.)")

### Linear Regression

Lets start by understanding the most commonly used algoritm in Regression called as Linear Regression.

> **Note:** Its recommended to only watch the first 16:00 minutes of the below video, but feel free to watch the rest for some advanced concepts.

[![Video: Linear Regression](https://img.youtube.com/vi/nk2CQITm_eo/0.jpg)](https://www.youtube.com/watch?v=nk2CQITm_eo "Linear Regression, Clearly Explained!!!")

## Regression Assignment
Once you have completed the Videos and Quiz above, let's try to get our hands dirty by implementing Linear Regression on a Real Life Example of Car Pricing Dataset.

**Dataset:** [Car Price Dataset](https://www.kaggle.com/datasets/hellbuoy/car-price-prediction)\
**Goal:** To predict values in `price` column

Task 1:
Train a Multivariate Linear Regression Model, and use it to predict car prices.

We will be using the Scikit-Learn (aka sklearn) python library to implement Linear Regression.\
Read more: [Linear Regression | sklearn](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)

For Task 1 we will be using `Dataset1-Train.csv` to train our model

High level Steps that you can follow:
1. Load the Train Dataset (`Dataset1-Train.csv`) in pandas dataframe
2. Split the dataframe into 2 different dataframes with first containing X variables and other containing y variables\
    X Dataframe: containing columns 'enginesize', 'curbweight', 'horsepower', 'carlength', 'carwidth'\
    y Dataframe: 'price'
3. Refer to the Examples on the scikit website on how to train a Linear Regression Model.
4. Once the Model is trained, use the model to predict the prices of cars in `Dataset1-Test.csv`
5. Calculate the R2 Score of the prediction and the values in `Dataset1-Test-prices.csv`

Target Score: > 0.6

## Solutions
View the Solutions only after you have completed all the exercies and quizes

Solutions: [Answers](./Answers.md) 
> **Note:** Don't jump to the answers directly without trying to solve/google/ask on your own.