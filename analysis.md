# Balkan Population Analysis

### Project Overview
This project analyzes population data from the Balkan region, focusing on identifying data inconsistencies and trends in the 2011 dataset.

### SQL Queries
```sql

USE mydb;
SELECT*FROM population
SELECT COUNT(*),  Country FROM population2011
GROUP BY Country 
HAVING COUNT(*)>= 2
ORDER BY COUNT(*);``` 