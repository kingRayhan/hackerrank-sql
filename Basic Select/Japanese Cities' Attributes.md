## Japanese Cities' Attributes
https://www.hackerrank.com/challenges/japanese-cities-attributes/problem

Query all attributes of every Japanese city in the  **CITY**  table. The  _COUNTRYCODE_  for Japan is  `JPN`.

**Input Format**

The  **CITY**  table is described as follows:

![](https://s3.amazonaws.com/hr-challenge-images/8137/1449729804-f21d187d0f-CITY.jpg "CITY.jpg")

# Solution
```sql
SELECT * FROM CITY 
WHERE COUNTRYCODE  = 'JPN'
```


> Written with [StackEdit](https://stackedit.io/).
