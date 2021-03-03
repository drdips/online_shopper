# Online Shopper Intention   

Flatiron Module 3 Project 
Contributors: Dipta Roy and Lauren Cunningham 

Dataset: Online Shoppers Intention dataset from Kaggle

https://www.kaggle.com/roshansharma/online-shoppers-intention


## Overview 

The objective of this project was to create a classification model from a dataset of our choosing and identify a problem we can solve. We used the Online Shoppers Intention dataset to see whether we could predict if a visitor to an online site will make a purchase or not. The dataset is from Turkey so there is an opportunity to provide recommendations to domestic online businesses as well as other countries looking to enter the market.


## Process 
1. See **data_cleaning.ipynb:** includes importing our dataset from kaggle, cleaning, analysis, visualizations and hypothesis testing.
2. See **feature_selection_modeling:** includes feature selection, dealing with class imbalance and modeling. 


## Libraries 
- Pandas
- Numpy 
- Matplotlib
- Seaborn
- Scipy
- Sklearn
- Imblearn 


## Modeling

**Feature selection**
- Lasso 
- F-test 
- RFE 

We ended up using the features from our F-test because it returned the most features.

**Modeling**
- Logistic Regression without balancing 
- SMOTE Logistic Regression
- Voting Classifier for SMOTE Log
- XG Boost with K Fold
- Random Forest with Grid Search

Our final model we chose is the Random Forest with Grid Search. It had the highest F1 score as well as the highest AUC on the ROC curve.


## Findings & Recommendations 

![Image](/visualizations/bounce_browser.png)

- Some browsers had a higher bounce rate, so we reccomend businesses focus on the UX/UI design of their site to ensure that its compatible with all browsers

![Image](/visualizations/seasonality.png)

- We found that fall months, in particular, November had the highest revenue. We assume that this is due to a lot of Turkish holidays falling within this time period. We recommend that businesses continue to offer seasonal products and deals throughout the entire year. 

![Image](/visualizations/specialday.png)

- In looking at whether the date is close to a special day, we found that that less visitors made less purchases. This is not what we expected, so we recommend that sites focus on making sure they have competitive deals and prices with other online businesses. 

![Image](/visualizations/visitortype.png)

- We found a significant difference between the new, returning and unrecognized visitor types with new visitors purchasing the most frequently. This was despite the fact that returning visitors spent more time on the site. There is an opportunity for more customer and brand loyatly. To do this businesses should personalize their shoppers experience with recommended products as well as a rewards system that offers benefits to returning visitors. 


 
