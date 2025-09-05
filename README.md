# Car_dataset


## Overview 
This is an detailed revenue report of the illustrious DAVE & DANN CAR COMPANY,The dataset that was used for this repository can be found in the description.
+ Total revenue by color
+ Total revenue by body style
+ Total revenue by dealer region
+ Total revenue by transmission
+ Total revenue by company
---
> This report is strictly about the revenue generated under cetain factors
---
## SQL queries
```sql
SELECT * FROM car_dataset;
```
```sql
--- Total revenue ---
SELECT SUM(price) AS Total_revenue
FROM car_dataset;
```
```sql
--- Total revenue by color ---
SELECT color,SUM(price) AS total_price
FROM car_dataset
GROUP BY color
ORDER BY total_price DESC;
```
```sql
--- Total revenue by body style ---
SELECT Body_style,SUM(price) AS total_price
FROM car_dataset
GROUP BY Body_Style
ORDER BY total_price DESC;
```
```sql
--- Total revenue by dealer region ---
SELECT Dealer_Region,SUM(price) AS total_price
FROM car_dataset
GROUP BY Dealer_Region
ORDER BY total_price DESC;
```
```sql
--- Total revenue by transmission ---
SELECT Transmission,SUM(price) AS total_price
FROM car_dataset
GROUP BY Transmission
ORDER BY total_price DESC;
```
```sql
--- Total revenue by company ---
SELECT Company,SUM(price) AS total_price
FROM car_dataset
GROUP BY Company
ORDER BY total_price DESC;
```
----
### PowerBI visualization
[Click here to view](https://ibb.co/1Cf12VD)
