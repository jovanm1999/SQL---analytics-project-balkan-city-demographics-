# Balkan Population Analysis

### Project Overview
This project analyzes population data from the Balkan region, focusing on identifying data inconsistencies and trends in the 2011 dataset.

### SQL Queries

# Balkan Population Analysis

I am analyzing this dataset to identify urban trends in the Balkan region.

### 1. Data Connection
First, I select the database and verify the data import.
```sql

USE mydb;
SELECT*FROM population;```

### 2. Analysis of Urban Concentration

Identifying how many countries have 2 or more cities within the most populous cities of ex-Yugoslavia list

```sql
SELECT COUNT(*),  Country FROM population2011
GROUP BY Country 
HAVING COUNT(*)>= 2
ORDER BY COUNT(*);``` 

