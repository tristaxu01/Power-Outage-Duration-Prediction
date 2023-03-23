---
layout: post
title: Background
---

Between January 2000 to July 2016, there were total of 1534 number power outrage that impacted at least 50,000 customers or caused an unplanned firm load loss of atleast 300 MW occured in United State. The largest power outage affected approximately 3.5 million people, and a maximum of 41,788 MW Peak Demand Power was lost during a single outage event. The focus of our website is to investigate the relationship between monthly electricity prices in the residential sector (labeled as "RES.PRICE" in the dataset) and power outages caused by intentional attacks. Specifically, we aim to determine whether regions with a top 25% residential electricity price are more likely to experience power outages caused by intentional attacks.

-----

# Framing the Problem 
### Prediction Problem
The aim of this project is to predict the duration of power outages in minutes, using previous major outage data from January 2000 to July 2016. This is a regression problem that will help local organizations and individuals take preventive measures to minimize losses before an unexpected power outage event occurs.

### Response Variable and Model Evaluation
Power outages can result in significant financial losses and negatively impact people's lives. To predict the quantitative data of the power outage duration in minutes, we will use external factors such as climate, geography, and local electricity information. To measure the ability of our model to predict quantitative data, we will use mean squared error. By doing so, we hope to provide accurate and useful information to help individuals and organizations prepare and prevent significant losses resulting from power outages.

### Feature Investigation
By the time of prediction, our team has thoroughly explored the data on major power outage events in the continental US and has collected basic information about each outage event, including location, occurrence time, regional information, etc. The data cleaning and investigation process has been documented on a [separate website](https://github.com/tristaxu01/Intentional-Power-Outage), which also explores the relationship between electricity prices and power outage causes. After the preparation process, we further explored the relationship between the outage duration and factors such as US state, state population, outage occurrence time, and climate region to improve the accuracy of our model.

# Baseline Model
### Feature Description
For the baseline model, our team selected four columns: "CLIMATE.REGION", "POPULATION", "MONTH", and "START.HOUR" extracted from the "OUTAGE.START (Y-M-D time)" column. During pipeline construction, we standardized the "POPULATION" column and one-hot encoded the rest of the features. Among the selected features, "POPULATION" is quantitative discrete data, "MONTH" and "START.HOUR" are quantitative ordinal data, and "CLIMATE.REGION" is categorical. We used one-hot encoding to transform "MONTH", "START.HOUR", and "CLIMATE.REGION" into quantitative nominal columns as model features.

### Feature Selection
We included the "POPULATION" column because greater population indicates urbanization and maturing infrastructure, making places with more population less likely to experience long power outages. 
* "POPULATION" column was included due to greater population indicating urbanization and mature infrastructure, which makes places with more population less likely to experience long power outages.
* "CLIMATE.REGION" was included as more certain climate regions are likely to experience extreme weather and longer power outages.
* "MONTH" feature is essential as different months correspond to national festivals and electric usage peaks.
* "Start hour" of the power outage was added to the model as outages starting at midnight may require more time to restore due to fewer resources available.

### Choice of Regressor
For the baseline model, we selected Random Forest Regressor because it can handle a large number of features, has lower overfitting risk compared to other models, and can model nonlinear relationships between features, which is useful for predicting outage duration. The algorithm also considers interactions between categorical and quantitative features, making it suitable for the diverse and complex data in this prediction problem. Overall, the Random Forest Regressor is a good choice for outage duration prediction due to its flexibility and ability to handle complex data.

### Performance Analysis
Based on the high RMSE value of around 5000, it seems that the current model is not accurate enough for practical use. One reason for this could be that the feature selection process was based solely on intuition, and the selected features may not be sufficiently informative to predict the duration of power outages. Additionally, the model's overall simplicity may not capture the complex relationships and interactions between the features and the outage duration. Therefore, it may be necessary to consider more advanced modeling techniques and more informative features to improve the model's accuracy.
