# Heart Disease Detection using ML

It is a classification problem where we will check whether the person's heart is healthy or not.

It's a really simple and basic project. We will be using Logistic Regression model.

### Notes : -
#### 1. `value_counts()` Function
We use this function to check the occurences of unique values of a particular column. 

In this case, we are trying to check how many patients have a healthy heart (represented by the *target* value of **0**) and how many have an unhealthy heart (represented by the *target* value of **1**)

#### 2. Creating the Feature DataFrame and Target Series
To do this, we are simply dropping the *Target* column from the dataset to get the Feature DF and just selecting the *Target* column for our Target Series.

#### 3. Splitting the data
Before we train the model, we need to split the data into 2 sets :-
1. Training set
2. Test or validating set.

To split the data, we are using the function `train_test_split()`.

We are passing 4 parameters in this function :-
1. The feature dataset
2. The target dataset
3. `test_size` : By default it's .25, which means 25% of the dataset will be used for testing and the other 75% for the training.
4. `random_state` : This is to make sure that our data split remains same during every execution.

#### 4. Training the model
Here, we are creating a model of `LogisticRegression()` class. 

We train, predict, and score the model in the same way we train Decision Tree model or Random Forest model (at least at this basic level :) ).

<br>


> This project was a complete walkthrough of this [tutorial](https://youtu.be/F_9gGyCs3YY?si=GDHr1nkJf4QHzUhG) by GFG.
