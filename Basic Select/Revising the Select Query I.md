## Revising the Select Query I
https://www.hackerrank.com/challenges/revising-the-select-query/problem

Query all columns for all American cities in  **CITY**  with populations larger than  `100000`. The  _CountryCode_  for America is  `USA`.

**Input Format**

The  **CITY**  table is described as follows:![CITY.jpg](https://s3.amazonaws.com/hr-challenge-images/8137/1449729804-f21d187d0f-CITY.jpg)


---
# Solution
```sql
SELECT * FROM CITY
WHERE COUNTRYCODE = 'USA'
AND POPULATION > 100000;
```

> Written with [StackEdit](https://stackedit.io/).
