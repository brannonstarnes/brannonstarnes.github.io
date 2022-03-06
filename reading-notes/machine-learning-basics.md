# Machine Learning Basics

## Data Types

- Numerical - the data are numbers and can be split into sub-categories:
  - Discrete - integers only
  - Continuous - are of 'infinite' value (such as the size of an item)

- Categorical - cannot be measured, but describe a value such as color or presence of a feature

- Ordinal - like categorical but can be measured. School grades are an example (A, B, C+)

## Mean, Median, Mode and Numpy

Get in an explore Numpy, which has many useful methods to find common statistical answers. 

```
import numpy

customer_ratings = [4,6,9,3,6,8,5,8,6,7,5,9,10,6,1]

average_customer_rating = numpy.mean(customer_ratings)

print(average_customer_rating)
```

## Standard Deviation

A number that describes how much spread is between a group of values.
- Low SD - values are close together
- High SD - values are spread further apart

For example, a SD of 0.9 means that ___most___ of the values fall within 0.9 of the median value.

In Numpy:
```
import numpy

customer_ratings = [4,6,9,3,6,8,5,8,6,7,5,9,10,6,1]

cust_ratings_standard_dev = numpy.std(customer_ratings)

print(cust_ratings_standard_dev)
```

## Fitting, DataFrames, Models

Fitting, or ___training___ data is a way to define decision-making based on certain values. For example, a house with two bedrooms may be predicted to sell 
at $250,000 vs a three bedroom at $320,000. 

This may be modeled using a decision tree.

The deeper the decision tree goes, the more accurate prediction can be made. 

### The First Step, Get to Know Your Data

Using the Pandas Library is a great way to get to know your data. 

### DataFrames

Think of DFs like a spreadsheet or an SQL table. 

### Steps to Building and Using a Model

- Define - What type of model? Decision tree? Other? Params?
  - ```from sklearn.tree import DecisionTreeRegressor```    
  - ```your_model = DecisionTreeRegressor(random_state=1)
- Fit - Capture the patterns from the data.
  -  ```your_model.fit(X,y)```
- Predict - State your hypothesis.
  - ```predictions = your_model.predict(X)``` 
- Evaluate - Determine accuracy of model's predictions.
  - Mean Absolute Error
    - ```from sklearn.metrics import mean_absolute_error```
    - ``` mean_absolute_error(y, predictions)``` 
