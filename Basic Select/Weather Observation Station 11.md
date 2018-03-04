
# Weather Observation Station 11
[Source](https://www.hackerrank.com/challenges/weather-observation-station-11/problem)

Query the list of CITY names from STATION that either do not start with vowels or do not end with vowels. Your result cannot contain duplicates.

The STATION table is described as follows:

![Station Table Structure][station]

> where LAT_N is the northern latitude and LONG_W is the western longitude.


## Answer
solved by [@KingRayhan](https://www.github.com/kingrayhan)
```sql
SELECT DISTINCT city FROM STATION WHERE
(city not like 'a%' or city not like '%a') or
(city not like 'e%' or city not like '%e') or
(city not like 'i%' or city not like '%i') or
(city not like 'o%' or city not like '%o') or
(city not like 'u%' or city not like '%u');
```

[station]: https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg "Station Table Structure"

