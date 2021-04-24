---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---


# Data Science Portfolio

<!-- ### _Paul's portfolio website showcasing some recent data science projects_ -->

## [Project 1: Housing Price Regression Model](https://github.com/pbeata/DSc-Training)
* Developed regression models using real estate data from the 2011 [Ames Iowa Housing Dataset](https://www.kaggle.com/marcopale/housing) on Kaggle: contains 2930 observations and 81 fields (features).
* Performed exploratory data analysis (EDA) with Pandas and Seaborn to understand the missing data and observe basic correlations among features
* Completed full data preprocessing by systematically handling all missing values in the raw dataset: removed outlier observations (3) and filled all null values with "0", "None", or a statistical estimate (e.g., mean), depending on the appropriate choice for each feature.
* Used Scikit-learn to develop an Elastic Net model employing Ridge and Lasso regularization
* Performed grid search cross validation to find optimal values of hyperparameters: results were alpha = 100 and l1_ratio = 1.0
* Achieved mean absolute error (MAE) of $14,195 and RMS error of $20,532, where the average house price in the dataset was $180,815 (relative MAE = 7.8%) 

![](/images/percent_nan_barplot.png)

