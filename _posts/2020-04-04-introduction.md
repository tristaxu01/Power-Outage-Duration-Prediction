---
layout: post
title: Background
---

Between January 2000 to July 2016, there were total of 1534 number power outrage that impacted at least 50,000 customers or caused an unplanned firm load loss of atleast 300 MW occured in United State. The largest power outage affected approximately 3.5 million people, and a maximum of 41,788 MW Peak Demand Power was lost during a single outage event. The focus of our website is to investigate the relationship between monthly electricity prices in the residential sector (labeled as "RES.PRICE" in the dataset) and power outages caused by intentional attacks. Specifically, we aim to determine whether regions with a top 25% residential electricity price are more likely to experience power outages caused by intentional attacks.

-----

# Framing the Problem 

Power outages are a common occurrence in the power network, and various factors can contribute to these events. As previously mentioned, power outages can result in significant financial losses and negatively impact people's lives. Predicting power outages can help local organizations and individuals take preventative actions to minimize losses before an unexpected event occurs. Our website explores data on major power outage events in the US continental and investigates the relationship between outage duration and factors such as US state, state population, outage occurrence time, climate region, and more using regression analysis. (The data cleaning process has been thoroughly documented on a [separate website](https://github.com/tristaxu01/Intentional-Power-Outage) that explores electricity prices and power outage causes.)

Our team aims to predict the quantitative data of the power outage duration in minutes based on external factors such as climate, geography, and local electricity information. To measure the ability of our model to predict quantitative data, we will use mean squared error. By doing so, we hope to provide accurate and useful information to help individuals and organizations prepare and prevent significant losses resulting from power outages.


