---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---


# Data Science Portfolio

<!-- ### _Paul's portfolio website showcasing some recent data science projects_ -->

## [Project 1: Housing Price Regression Model](https://github.com/pbeata/housing_price_model)

View Notebooks in Browser: [Data Preprocessing](projects/housing_data_preprocessing.html) \| [Regression Model](projects/housing_data_regression.html) |

* Developed regression models using real estate data from the 2011 [Ames Iowa Housing Data](https://www.kaggle.com/marcopale/housing) on Kaggle containing 2930 observations and 81 fields (features)
* Performed exploratory data analysis (EDA) with NumPy, Pandas, and Seaborn to understand the missing data and observe which features have strong correlations with the final sale price 
* Performed data preprocessing by systematically handling all missing values in the raw data set: removed outlier observations (3) and filled all null values with either "0", "None", or a statistical estimate (e.g., mean), depending on the appropriate choice for each feature.
* Used Scikit-learn to develop regression models using an elastic net model, ridge and lasso regularization, ordinary linear regression, and a random forest regressor 
* Performed grid search cross validation to find optimal values of hyperparameters
* Employed lasso regression and achieved mean absolute error (MAE) of $14,191 and RMS error of $20,554, where the average house price in the data set was $180,815 (relative MAE = 7.8%) 

![](images/house_feature_correlation.png)

<!-- ![](images/linear_house_model_results.png) -->


## [Project 2: Client Churn Predictor](https://github.com/pbeata/client_churn_predictor)

View Notebook in Browser: [Classification Models](projects/client_churn_model.html) |

* Developed classification models using customer data from a telecommunications company containing 7032 observations (rows, each representing unique customers) and 21 fields (features + target)
* Using historical data about the customers, such as their tenure with the telecom service, their contract type, etc., and data regarding customer churn, we built classifiers for predicting future customer churn
* Performed exploratory data analysis to understand the relationships between contract type, charges (fees), services, and tenure, and how these factors affected the company's churn rate
* Used cohort analysis to investigate the differences among cohorts: we found that customers on a one-year or a two-year contract were much less likely to churn than customers who are on month-to-month contracts
* Employed various tree-based methods, such as Single Decision Trees, Random Forests, AdaBoost classifier, and Gradient Boosting, as well as Support Vector Machines and K-Nearest Neighbors to perform this classification task
* Using a grid search with 10-fold cross validation on the AdaBoost classifier, we found that the optimal learning rate and number of estimators were 0.25 and 100, respectively: this leads to an accuracy of 82% and similar recall (between 80% and 83%) 

![](images/roc_curve.png)
