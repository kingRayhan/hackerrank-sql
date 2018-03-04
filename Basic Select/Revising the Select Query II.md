## Revising the Select Query II
https://www.hackerrank.com/challenges/revising-the-select-query-2
Query the names of all American cities in  **CITY**  with populations larger than  `120000`. The  _CountryCode_  for America is  `USA`.

**Input Format**

The  **CITY**  table is described as follows:![CITY.jpg](https://s3.amazonaws.com/hr-challenge-images/8137/1449729804-f21d187d0f-CITY.jpg)

---
# Solution
```sql
Select name from city 
where countrycode = 'USA'
and population > 120000;
```
