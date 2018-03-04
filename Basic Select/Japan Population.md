## Japan Population
Source: https://www.hackerrank.com/challenges/japan-population/problem

Query the sum of the populations for all Japanese cities in  **CITY**. The  _COUNTRYCODE_  for Japan is  **JPN**.

**Input Format**

The  **CITY**  table is described as follows:

![](https://s3.amazonaws.com/hr-challenge-images/8137/1449729804-f21d187d0f-CITY.jpg "CITY.jpg")

---
# Solution
```sql
select sum(population)
from city
where COUNTRYCODE = 'jpn'
```
