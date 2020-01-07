---
layout: post
title:  "Employee Performance and Attrition Analytics"
date:   2020-01-07 13:26:44 +0530
categories: general windows
layout: post
tag:
- Human Resource
- Employee Satisfaction
- Attrition
- HR Analytics
star: true
author: archit
---

## 1. Introduction & Business Understanding 
Go to this [page](https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset) to download 'IBM Attrition Dataset'


At any given point in time, about 50% of the employees in an organization are considering changing of employer according to a statistic shared by Gallup. Employee attrition is a huge problem faced by organizations because every outgoing employee takes countless hours of training and other resources invested in him or her by the employer. By understanding what variables in terms of employee characteristics, work experience, etc. increase the probability that an employee would leave the organization, the company can realize significant savings monetary and time wise. This is precisely what we are trying to solve here – find the variables (or predictors) that can influence or determine whether an employee would leave the organization or not. Our project falls under the category of Human Resource (HR) Analytics. 

You will be required to signup and login to download this
 ![Signin](https://www.dropbox.com/s/lo2fjnqbbd9y5so/Capture-2.PNG?dl=1)



## 2. Data Description 

The dataset is fictional and has been created by IBM data scientists to understand the phenomenon of Attrition.  It contains a total of 35 variables in which column ‘Attrition’ is the one we intend to predict. In this case, ‘Attrition’ is our target (or Dependent) variable and the leftover 34 variables, which includes the likes of Gender, Education, Department etc., are predictor (or Independent) variables. ‘Attrition’ is a binary variable, only taking in “Yes” (1) or “No” (0) as values. The total number of rows in the dataset is 1470. Including the column Attrition, there are 21 categorial variables and the rest are continuous in nature. Majority of the categorical variables are encoded in the following manner:  

1 = Low  2 =  Medium 3 = High  4 = Very High 

For education: 1 = Below College 2 = College 3 = Bachelor  4 = Master  5 = Doctor 


## 3. Data Cleaning and Variable Categorization 

We used the “MICE” package to whether or not there are NULL values in the dataset. The test revealed there are none. After studying the structure, we found 3 columns ('Over18', 'EmployeeCount', and 'Standard Hours') that are constant in nature. These columns were dropped from our analysis. We excluded the column ‘EmployeeNumber’ as well, because it doesn’t add value. Finally, based on the data type of the remaining 30 variables (excluding the target variable), we classify them into 6 categories as listed below: 

## 4. Exploratory Data Analysis 

Because our target variable is a categorical one (Yes/No), scatterplots essentially wouldn’t be useful here. Thus, we’ll make judicious use of bar charts, line charts, histograms and mosaic plots to convey our insights. 

![Login](https://www.dropbox.com/s/ma6w6h9h6hjc1l8/Capture-8.PNG?dl=1)

Now after this you can directly use SQL commands or if you prefer, create new user to use.

![SQL Command Line Usage](https://www.dropbox.com/s/oj28p2wp6gw0r9r/Capture-9.PNG?dl=1)

### 1. Attrition Distribution On the Basis of Personal Background 

First, we explore the attrition distribution based on personal information. There are 237 employees who left the company, which amounts to 16.1% of the total sample. This quite high as compared to the industry standard of 10% (anything above it is considered problematic).  
The age distribution of people who left the company concentrates on people that are between 25-35 years old. As the age goes up, people show less tendency to leave the company. There is no major difference of the attrition distribution between females and males. According to the department distribution, it shows that employees from the R&D and Sales department have higher chances to leave the company. 

### 2. Attrition Distribution on the Basis of Income  

Salary is the most (or at least one of the most) motivating factors for an employee. We start our analysis with Monthly Income.

As witnessed from the boxplot, the average monthly income stands at around $6500 and the maximum value goes till $20000. There are some outliers but we’ll keep them untouched as people do earn (or are at least capable of earning) that kind of money.  

Next, we further our visualization by plotting a histogram of Monthly income dividing between gender. We suspected that there might be a difference in attrition between male and female when salary is equal, but as evident from the graph, this is clearly not the case. The attrition is highest when the employee is earning in the range of $1000-$7000, which is expected of the range in question. 

Moving on, we plotted the interaction of average of Monthly income with level of Education. As suspected, people who left the company had lower average income across all education levels as compared to people who didn’t leave the company. This directly points out to the importance of salary in Attrition. 

Next, we investigated % hike and divided that among Male-Female. As witnessed from the graph, lower the % hike, higher is the attrition. But there is no considerable difference in the ratio of Attrition when we differentiate amongst male female which indicates that Gender might not be a strong factor for determining Attrition. 

![Attrition Distribution](https://github.com/architgupta33/architgupta33.github.io/blob/master/assets/images/1.png)

## 4. Exploratory Data Analysis 

## 4. Exploratory Data Analysis 

*This post is inspired from the questions of my batchmates so major credits goes to them*
