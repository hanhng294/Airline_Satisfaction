# Analysis and Prediction of airline customer satisfaction

Programming language: Python
Packages: pandas, numpy, matplotlib, seaborn, scipy.stats, sklearn
link to dataset: https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction

- Task Description
- Dataset Description
- Exploratory Data Analysis
- Data Handling
- Predction model
- Important features

## Task Description
Airline satisfaction has been an alarming issues for the past few years with customer complaint about delays or in-flight services.
I used the dataset that consists of passenger satisfaction survery, as well as their demographic information and flight attributes. 
The goal of this case study is to predict customer satisfaction and examine important attributes that affect the outcome in order
to recommend areas of focus for improvement.

## Dataset description
- The target attribute is satisfaction with 2 categories: neutral or dissatisfied and satisfied.
- Other attributes include: gender, customer type, age, type of travel, class, inflight wifi service, departure/arrival time,
  ease of online booking, gate location, food and drink, online boarding, seat comfort, inflight entertainment, on-board service,
  leg room service, baggage handling, check-in service, inflight service, cleanliness, departure delay in minutes, arrival delay in minutes

## Exploratory Data Analysis
- I examined the dataset by looking at summary of information as well as using visualizations (bar chart) for exploring distributions
- I used pairplot to cover all attributes and correlation plot combined with heatmap to explore correlations.

## Data Handling
- Due to high number of attributes, I dropped some columns that have low correlation with target attribute (gender) or has high correlation with
another attribute (I dropped arrival delay in minutes as it is highly correlated with Departure delay in minutes)

## Prediction Model
I used SVM and Catboost to train on training dataset and predict satisfaction on test set. The results are discussed in 

## Important features
I used the get_feature_importance in catboost to uncover important factors that contribute to customer satisfaction. This can help airline
companies to understand what are the deciding factors that lead to level of customer satisfaction and helo narrow down neccesary actions.
Important features are discussed in: 
