# Bike Sharing Prediction

## Context

Using a dataset from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/bike+sharing+dataset) that contained information about hourly and daily counts of rental bikes in Washington DC, I wanted to build a model that could predict the number of rental bikes being used.

## Tools Used

The tools, libraries and models that I used for this project were:

  * Pandas
  * NumPy
  * Matplotlib
  * Seaborn
  * [Plotly](https://plotly.com/python/)
  * Feature Scaling (MinMaxScaler and StandardScaler)
  * Linear Regression (OLS)
  * [Poission Regression Model](https://towardsdatascience.com/an-illustrated-guide-to-the-poisson-regression-model-50cccba15958)
  * [Negative Binomial (NB) Regression Model](https://towardsdatascience.com/negative-binomial-regression-f99031bb25b4)
  
## Process

Before creating machine learning models for this project, I did some EDA as well as data cleaning and data preprocessing:
  * Dropping unnecessary columns;
  * Identifying columns with high correlation between each other;
  * Encoding categorical variables;
  * Feature Scaling.
  
Several approaches were applied for this project, in order to improve the Adjusted R-Squared and reduce the Mean Squared Error. Of all the models that were built, I would mention the **Poisson Regression Model** and the **Negative Binomial Regression Model** as the ones with the most interesting results.
These two models are the most appropriate for these kinds of datasets, where you are trying to predict count-based data on a certain time period. In this case, we are trying to predict **the number of bikes per hour**.

You can check the [python file](https://github.com/tmcdonald92/Bike-Sharing-Prediction/blob/main/Regression%20Analysis.ipynb) for more information on these models and how they were built.
