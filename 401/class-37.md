# Machine learning

Machine learning allows for computers to recognize patterns in data, often so they can make predictions or decisions.

## overview

### key terms

- Model - a set of patterns learned from data
- Algorithm - a specific machine learning process used to train a model
- Training data - a dataset for an algorithm to learn a model
- Test data - different dataset used to evaluate the performance of a model
- Features - Variables (columns) in the dataset use to train the model
- target variable - specific variable for which you are trying to predict
- observations - data points (rows) in the dataset

### tasks

Machine learning has more than these two categories of taskes, but the main two are supervised learning, where you have a target variable, and unsupervised learning, where you do not.

### 3 elements of great machine learning

1. a skilled chef (human guidance)
2. fresh ingredients (clean, relevant data)
3. don't overcook it (avoid overfitting)

### core steps

1. exploratory Analysis
2. data cleaning
3. feature engineering
4. algorithm selection
5. model training

---

## Exploritory Analysis

This is where you get to know your dataset. Its a critical step, but should not be drawn out. Some key questions you might ask:

- How many observations? (rows)
- How man features (columns)
- What data types do I have?
- Do I have a target variable?
- Is missing data going to be an issue?
- Is the data arranged in a way that makes send?
- Do the values make sense?

Plotting numerical data can be useful for quick visualisations. You may be able to spot outliers or odd distributions that don't make sense, and require investigation during data cleaning.

## Data Cleaning

In machine learning there is a saying, garbage in, garbage out. So lets not feed garbage into our algorithms.

Remove unwanted observations. This includes duplicate or irrelevent observations.

Fix structural errors, such as typos and capilization, mislabeled classes.

Filter out unwanted outliers. But make sure that they are actually unwanted. Sometimes outliers are actually critical information to consider in your machine learning.

Handle missing data. This is tricky, and can include dropping observations or sometimes being missing is the actual important part. Don't just fill in the data with the mean, as that will just reinforce the trends, without adding any actual data.

## Feature engineering

Look for interaction feature, that is to say two or more features that can be combined in a useful way.

Combine sparse classes (if it makes sense to do so)

Removed unused features

## Algorithm Selection

Regularized regression

1. Lasso regression - penalizes the absolute size, can reduce coefficients to 0, which can remove features
1. Ridge regression - penalizes the square of cooefficients, so feature coeffciencts can approach 0
1. Elastic-net - tunes between the prior two

Decision Trees are better for non-linear relationships between features, but are prone to overfitting.

1. Random forests - use a large number of string decision trees, to smooth out the differences between them
1. Boosted trees - use weak decision trees (maximum depth contrained), which try to correct the tree that came before.

## Model Training

Think of your dataset as a limited resource. You can spend some of it to train your data, and you can spend the rest to evaluate the resulting model, but you can't soend any of it on both.

[<-- Back](../README.md)
