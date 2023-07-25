
# Retail Sales Prediction
Predicting sales of a major store chain Rossmann


![Logo](https://www.rossmann.de/medias/T33-Kat-50Jahre-Jubi-Geschichte-Laden-heute-01-896x400.png?context=bWFzdGVyfHVwbG9hZHw0OTEzNTZ8aW1hZ2UvcG5nfGgzOS9oNWMvMzUwNTA0NzA3Njg2NzAvVDMzX0thdF81MEphaHJlX0p1YmlfR2VzY2hpY2h0ZV9MYWRlbi1oZXV0ZV8wMV84OTZ4NDAwLnBuZ3wxZjk3MTViNGZhZjExNDFhOTk0YjI3MjU0MzFjNzkxYTU0MjUxY2ZlNDBkMDcwOWE2MzQ2MDVkMjI5YWMwNjg3&width=1408&auto=webp&quality=40&format=webply)


## Problem Description

Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.
You are provided with historical sales data for 1,115 Rossmann stores. The task is to forecast the "Sales" column for the test set. Note that some stores in the dataset were temporarily closed for refurbishment.


## EDA Strategy

My strategy to solve this challenge was:

    Step 01: Data Description: Use statistics metrics to identify data distributions.

    Step 02: Feature Engineering: Derive new attributes based on the original variables to better describe the phenomenon that will be modeled.

    Step 03: Exploratory Data Analysis: Explore the data to find insights and better understand the impact of variables on model learning.

    Step 04: Feature Selection: Selection of the most significant attributes for training the model.

    Step 05: Machine Learning Modelling: Machine Learning model training.

    Step 06: Hyperparameter Fine Tunning: choose the best values for each of the parameters of the model selected from the previous step.

    Step 07: Convert Model Performance to Business Values: Convert the performance of the Machine Learning model into a business result.
## Dataset

    Rossmann Stores Data.csv - historical data including Sales
    store.csv - supplemental information about the stores

1. Id - an Id that represents a (Store, Date) duple    within the test set
2. Store - a unique Id for each store
3. Sales - the turnover for any given day (this is what you are predicting)
4. Customers - the number of customers on a given day
5. Open - an indicator for whether the store was open: 0 = closed, 1 = open
6. StateHoliday - indicates a state holiday. Normally all stores, with few exceptions, are closed on state holidays. Note that all schools are closed on public holidays and weekends. a = public holiday, b = Easter holiday, c = Christmas, 0 = None
7. SchoolHoliday - indicates if the (Store, Date) was affected by the closure of public schools
8. StoreType - differentiates between 4 different store models: a, b, c, d
9. Assortment - describes an assortment level: a = basic, b = extra, c = extended
10. CompetitionDistance - distance in meters to the nearest competitor store
11. CompetitionOpenSince[Month/Year] - gives the approximate year and month of the time the nearest competitor was opened
12. Promo - indicates whether a store is running a promo on that day
13. Promo2 - Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating
14. Promo2Since[Year/Week] - describes the year and calendar week when the store started participating in Promo2
15. PromoInterval - describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store
## Conclusion

Acheived MAPE of 5.65% and MAE = $376 showing predictions of model is higly accurate for the sales forecast. Generated insights by EDA and feature importance provide valuable tools to decide the amount of budget and inventory for upcoming sales.
## Dataset

    Rossmann Stores Data.csv - historical data including Sales
    store.csv - supplemental information about the stores

1. Id - an Id that represents a (Store, Date) duple    within the test set
2. Store - a unique Id for each store
3. Sales - the turnover for any given day (this is what you are predicting)
4. Customers - the number of customers on a given day
5. Open - an indicator for whether the store was open: 0 = closed, 1 = open
6. StateHoliday - indicates a state holiday. Normally all stores, with few exceptions, are closed on state holidays. Note that all schools are closed on public holidays and weekends. a = public holiday, b = Easter holiday, c = Christmas, 0 = None
7. SchoolHoliday - indicates if the (Store, Date) was affected by the closure of public schools
8. StoreType - differentiates between 4 different store models: a, b, c, d
9. Assortment - describes an assortment level: a = basic, b = extra, c = extended
10. CompetitionDistance - distance in meters to the nearest competitor store
11. CompetitionOpenSince[Month/Year] - gives the approximate year and month of the time the nearest competitor was opened
12. Promo - indicates whether a store is running a promo on that day
13. Promo2 - Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating
14. Promo2Since[Year/Week] - describes the year and calendar week when the store started participating in Promo2
15. PromoInterval - describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store
## Screenshots

(https://drive.google.com/file/d/1xgXRQSPrgslkScJThjmDSpJ1t6HNgH74/view?usp=drive_link)

