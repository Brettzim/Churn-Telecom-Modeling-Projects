# Churn Telecom Modeling Projects
![SyriaTel_logo](./picture/SyriaTel_logo.jpeg)

Phase 3 Flatiron project developing ML models and predicts for Syria Tel

## Project Overview
This repository analyzes the data on SyriaTel’s customer churn to create machine learning classification models capable of predicting if a customer will churn or not. Our objective is to create a model using the customer churn data in SyriaTels’ customer database. The goal of our model is to have a high F1 score and Recall scores, so we know that our predictions are meaningful to the situation. By using different machine learning techniques, we were able to identify if a customer will churn, making our model a useful tool for the phone company interested in allocating its resources to customers. 
 
## Business Problem
We are an independent company audit firm hired by SyriaTel to investigate opportunities to increase customer retention by predicting customer loss from analyzing past data. We aim to provide a model highly successful at identifying if a customer will end their relationship with SyriaTel. The company can then take actionable steps to reduce their deficit.

## The Data
This project uses the SyriaTel Customer Churn dataset. The dataset includes customers that do business with SyriaTel in all 50 states. The descriptions of the dataset's columns are shown below.

* State - a State abbreviation. The state location of the customer.
* Account Length - How long the customer has been with the company.
* Area code - Area code of the customer.
* Phone number - Phone number of the customer.
* International plan - true if the user has the international plan, otherwise false.
* Voicemail plan - true if the user has the voicemail plan, otherwise false.
* Number vmail messages - the number of voicemail messages the customer has sent.
* Total day minutes - total number of minutes the user has been in calls during the day.
* Total day calls - total number of calls the user has done during the day.
* Total day charge - total amount of money the user was charged by the Telecom company for calls during the day.
* Total eve minutes - total number of minutes the user has been in calls during the evening.
* Total eve calls - total number of calls the user has done during the evening.
* Total eve charge - total amount of money the user was charged by the Telecom company for calls during the evening.
* Total night minutes - total number of minutes the user has been in calls during the night.
* Total night calls - total number of calls the user has done during the night.
* Total night charge - total amount of money the user was charged by the Telecom company for calls during the night.
* Total intl minutes - total number of minutes the user has been in international calls.
* Total intl calls - total number of international calls the user has done.
* Total intl charge - total amount of money the user was charged by the Telecom company for international calls.
* Customer service calls - number of customer service calls the user has done.
* Churn - true if the user terminated the contract, otherwise false.

## Data Cleaning

The data here started out with no null values, and data types that aligned with the supposed data values. After some correlation analysis, we decided to remove all columns related to charge, as every charge column had an almost a 1:1 correlation with its minutes column. We also removed the “phone number” and “number vmail messages” columns. In order to turn the object columns into usable numerical data, we used a one hot encoder on the “Voice mail plan”, “International plan”, and "State" columns. We used a label encoder on the target column “Churn”.
 

 
