# HomeCredit-Project

## Summary of business problem & objective:
Home Credit wishes to expand financial services to the unbanked population, where traditional credit history is limited or even non-existent. To assess creditworthiness, they supplement loan applications with alternative data such as transaction records and telecom behavior. This is commonly referred to as "telco data"

The primary business objective is to predict the likelihood of loan default. 0 indicates No default and 1 represents at least one late payment. Accurately predicting defaults will help Home Credit minimize losses and promote financial inclusion while ensuring responsible lending. This project aims to build a predictive model to assess clients loan repayment ability using available data

## Solution to the business problem
Our solution to this problem is to develop a model that can essentially predict loan defaulters compared to non defaulters. This will help home credit assess loan applications to minimize defaults which lead to losses. Mitigating defaults will increase profits and establish business sustainability. Individually I created a preliminary logistic model in the individual notebook. With my group we created a Catboost model. The catboost model was able to capture non linear data and had better performance metrics than the logistic regression model.

## Contributions to the Project
I have made several contributions to the project such as:
KNN modelling, Hyperparameter Tuning (GridSearchCV/RandomSearchCV), Confusion matrix implementation, ROC curve, adding group members code for bureau analysis onto the final model. Fixing CNT_Children variable via capping. Creating function to cap numeric outliers within +/- 3SD of mean. Pasting team functions onto the final file. Adding teams summary statistics and data exploration graphs.

## Business Value of the solution
The initial notebook (individual version) was able to identify which predictors lead to default namely: age, credit scores, duration of the change in phone numbers. 
The group notebook captured simillar predictors, but was more focused on enhancing the predictive power of the model by downsampling and feature engineering and using catboost. This new and refined model delivers business value to HomeCredit as it allows them to accurately assess defaulters/non defaulters with more confidence. 

## Difficulties encountered in the Group Notebook
In the group notebook we had some difficulties in regards to performing all the data transformation together and have it flow sequentially. Such as scaling, downsampling and using dummie variables. To mitigate this, I will recommend my group to use pipeline in the next project. Pipeline allows one to perform several steps at once and you can clean your data all together. Having a neat notebook is challenging for a group and pipeline makes that easier. Ultimately I realized that reading someone elses code could be a challenge too. Therefore, it is important to leave comments to describe steps taken. Also finding the best model was a challenge. There are multiple models and each of them have their own advantages/disadvantages. Perhaps in a future project we can use pipeline and iterate models via a for-loop to quickly create multiple models.


## What I learned
This project was quite essential in grasping the concepts of using machine learning in Python. Personally, I learned that it might not be best to start cleaning the data right away. We should explore it, afterwards split the data and then clean the data. Not splitting the data before cleaning can cause data leakage. Furthermore, I learned how important it is to focus on exploring the data accurately. Its easy for one to devote their attention towards the model, however the explanatory phase is just as essential. Having outliers, null data, dirty data can affect the models results. Therefore, data cleaning must never be neglected. Also, I learned more about scikit learn and its capabilities. I will continue to use scikit learn when I can for Machine learning.



