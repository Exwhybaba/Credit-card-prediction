# Credit-card-prediction
## Introduction

The manager at the bank is concerned about the increasing number of customers leaving their credit card services. In response to this problem, the bank wants to proactively approach the customers who are likely to churn and provide them with better services to prevent them from leaving. To address this issue, we have obtained a dataset from https://leaps.analyttica.com/home that contains information about 10,000 customers, including their age, salary, marital status, credit card limit, credit card category, and other related features. The aim of this report is to develop a model that can predict which customers are likely to churn.

## Data Exploration:

The dataset contains 10,127 observations and 23 features, out of which we have identified 16 features that are relevant to our analysis. The target variable in this dataset is whether a customer has churned or not. We observed that only 16.07% of customers have churned, making it a class imbalance problem. We need to keep this in mind while selecting our evaluation metrics and building our model.

We conducted exploratory data analysis to better understand the data. We found that the average age of customers in the dataset is 46 years, with a standard deviation of 8 years. The average credit card limit is $4,549. We also observed that the majority of customers have an average credit card limit of $30,283.45 and fall into the Platinum credit card category.

## Data Preprocessing:

We performed several data preprocessing steps to prepare the data for model building. First, we checked for missing values and found that there were none. Next, we converted categorical variables into numerical variables using Ordinal encoder to make them suitable for machine learning algorithms. We also rescaled the numerical features to ensure that they are on the same scale and normalized to ensure they are normally distributed. We used recursive feature elimination to eliminate unnecessary features that constitute noise to our model and discovered that only 7 features are more relevant to our prediction. We used K-fold cross-validation to split our data into train and test data, ensuring more reliable evaluation.

## Model Building and Evaluation:

After evaluating various machine learning algorithms, we found that the KNearest Neigbour algorithm performed the best in predicting which customers are likely to churn. The KNearest Neigbour algorithm had an accuracy of 92.194%, while Logistic Regression had an accuracy of 89.921%

## Conclusion:

Our analysis demonstrates that it is possible to predict customer churn with a high degree of accuracy using machine learning algorithms. The bank can use this model to identify customers who are likely to churn and provide them with better services to prevent them from leaving. Overall, our analysis provides valuable insight into how machine learning can be used to address business problems and improve customer satisfaction.


