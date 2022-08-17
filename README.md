# Bike-Sharing-Demand
## Introduction
Renting bike is a booming business due to various
reasons. According to the data compiled by the team behind
the Medina bike sharing map, there are currently over 3,000
bike share systems in cities around the globe Bike sharing
systems are a means of renting bicycles where the process of
obtaining membership, rental, and bike return is automated via
a network of kiosk locations throughout a city. Using these
systems, people are able rent a bike from a one location and
return it to a different place on an as-needed basis.
The benefits of bike sharing schemes include transport
flexibility, reductions to vehicle emissions, health benefits,
reduced congestion and fuel consumption, and financial savings
for individuals.

## Problem Statement
Rented bikes are introduced in many urban cities for the enhancement
of the mobility comfort. Our objective is to predict the count of bikes
required at each hour throughout the day so that bikes are accessible
to the public at right time and thus lessening the waiting time.

## Exploratory Data Analysis
The main purpose of EDA is to detect any errors, outliers as well as to
understand different patterns in the data. It allows Analysts to
understand the data better before making any assumptions. The
outcomes of EDA help businesses to know their customers, expand
their business and take decisions accordingly.

## Data Pre-processing
Data pre-processing is a process of preparing the raw data and making
it suitable for a machine learning model. It is the first and crucial step
while creating a machine learning model.
We performed the data pre-processing in following manner:

1. We looked for the null or duplicate values and found none in the
given dataset
2. there were outliers in many features of our dataset so treated the
outliers by removing them and filled the NaN values with mean of the
respective column
3.We converted the categorical features into numeric by creating
dummy variables.

We created dummy variables for season, day of the week, year,
month, holiday and functioning day columns
5. We checked the correlation of features with our target variable and
removed the highly correlated variables. The most highly correlated
variables were Dew point temperature with a positive correlation of
0.91. We dropped snowfall and rainfall as well due to presence of NaN
values after getting rid of outliers.

## Models Used
1. Linear Regression 
2. Lasso Regression
3. Decision Tree
4. Random Forest

## Challenges faced
• Pre-processing the data was one of the challenges we faced
which includes removing highly correlated variables from the
data so as to not hinder the performance of our regression
model.
• Exploring all the columns and calculating VIF for
multicollinearity was challenging because it might decrease the
model’s performance.
• Selecting the appropriate models to maximize the accuracy of
our predictions was one of the challenges faced.

## Conclusion 
We performed the EDA and understood the features which affect
most to bike sharing demand. Further we converted our data into a
machine-readable format so can predict the count of rented bikes
required at a particular hour throughout the day. We cleaned our data
and fit the model.

We concluded the following points:
• Maximum numbers of bike are rented during the year 2018.
• Demand of the rented bike is maximum during functioning day
and no holidays.
• Summer seasons is the season of highest rented bikes whereas
winter has least number of bikes rented.
• Peak time for renting bikes is between 7 to 9 am in the morning
and 5 to 7 pm in the evening. This could be due to the fact that
maximum bikes are rented by office going people.
• The model that performed best on the given dataset is Random
Forest with an r2 score of 0.83.
• Linear regression performed the worst out of all the models with
an r2 score of just 0.58.
• Decision tree is also performed really good with an r2 score of
0.80
