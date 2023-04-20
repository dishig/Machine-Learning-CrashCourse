# Chapter 2: Datasets Pre-processing

Great Job on completing the previous chapter! In this chapter we will add more features to our cars dataset and use them to improve our regression score.

Today we will be using the extended version of the Car Pricing Dataset: [Dataset2.csv](./Dataset2.csv)

## Agenda
1. Handling Categorical Features
2. Handling missing data
3. Advanced Regression and interpretting results

## Handling Categorical Features

As we saw in previous chapter, Linear regression builds a relationship between a dependent variable (the outcome or target variable) and one or more independent variables (the input or feature variables). However, linear regression is designed to work with numerical data, which means it can only take numerical features as input.

Numerical features are variables that represent quantities and can be measured on a continuous scale, such as age, height, weight, or temperature. These variables have numeric values that can be directly used in mathematical calculations.

On the other hand, categorical features are variables that represent categories or groups, such as gender, color, or city. Categorical features have discrete values and do not have a numerical order or scale. For example, the categories "male" and "female" in the gender feature cannot be directly used in mathematical calculations by linear regression.

To use categorical features in a linear regression model, they need to be converted into numerical features. This process is called encoding or feature encoding. 

There are several common methods to do this, such as:

1. **Label encoding**: Assigning a unique numeric label to each category in the categorical feature. For example, converting "male" to 0 and "female" to 1.

2. **One-Hot encoding**: Creating binary (0/1) dummy variables for each category in the categorical feature. Each dummy variable represents whether a particular category is present or not. For example, creating two dummy variables "is_male" and "is_female" with values 0 or 1 to represent gender.

Watch this video by DataCamp to get a better understanding of the concept and its implementation.

[![Video: Python Tutorial: Dealing with categorical features](https://img.youtube.com/vi/WXHLLO4FnZs/0.jpg)](https://www.youtube.com/watch?v=WXHLLO4FnZs "Python Tutorial: Dealing with categorical features")

The methods mentioned in the video can also be implemented directly in Sklearn using in-built functions `preprocessing.OneHotEncoder` and `preprocessing.LabelEncoder` in the [sklearn.preprocessing class](https://scikit-learn.org/stable/modules/classes.html#module-sklearn.preprocessing).

### Exercise

1. Identify the Categorical and Numerical columns from the above [Dataset2.csv](./Dataset2.csv).
2. Identify which techniques are most suitable for each categorical columns.

## Handling missing data

Most real world dataset require some pre processing before they can be used in the models. In fact, its believed that most data scientist spend 60% of their time pre processing the data before they can start with model experimentations.

One of the common problems seen in the data set is "missing values", in which certain values of a column are blank of `NaN` (Not a Number)

The following video explores ways on how missing values can be rectified.

[![Video: Handling Missing Values in Pandas Dataframe | GeeksforGeeks](https://img.youtube.com/vi/uDr67HBIPz8/0.jpg)](https://www.youtube.com/watch?v=uDr67HBIPz8 "Handling Missing Values in Pandas Dataframe | GeeksforGeeks")

### Exercise
1. Identify which columns in the dataset have missing values.

## Assignment 1: Advanced Regression 

**Goal:** To predict values in `price` column

Task 1:\
Train a Multivariate Linear Regression Model, and use it to predict car prices. 
- Use all the columns given in the dataset to train the model.
- Find and impute (fill) the missing values in the dataset if any

> Note: You can reuse same Linear Regression Model code from the last chapter 

For Task 1 we will be using `Dataset2.csv` to train our model

High Level Steps that you can follow
1. Load the Train Dataset (`Dataset2.csv`) in pandas dataframe
2. Fill the missing values
3. Convert the categorical variables into numerical variables
4. Train-test split the model into 80%-20% split
5. Train the Model and calculate the r2 score.

## Assignment 2: Interpreting features and feature selection

As you might have seen in the previous assignment, we had over 10+ features which we had to input into linear regression. But in real world, more features doesn not always mean better model.

So its neccessary to identify the top useful features and train the model only with those model

One common technique is to use Pearson Correlation to calculate to correlation of each of the feature to the target variable. You can learn more about it in the below video.

[![Video: 12 Machine learning in python || Correlation Analysis and Feature Selection](https://img.youtube.com/vi/BCuIq206lrA/0.jpg)](https://www.youtube.com/watch?v=BCuIq206lrA "12 Machine learning in python || Correlation Analysis and Feature Selection")

Task 2:\
Identify the top important features are retrain the model using only the selected features. Try taking Top 3, Top 5, Top 10, Top 15 feature columns and train the model for each of those feature set.

For Task 2 we will be using the same `Dataset2.csv` to train our model. Reuse the preprocessing steps done in Task 1 to convert Categorical variables and to impute missing values.

Compare the R2 scores for Top 3, Top 5, Top 10, Top 15 feature columns and draw conclusion.

## Solutions
View the Solutions only after you have completed all the exercies and quizes

Solutions: [Answers](./Answers.md) 
> **Note:** Don't jump to the answers directly without trying to solve/google/ask on your own.
