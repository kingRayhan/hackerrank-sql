## Weather Observation Station 3
https://www.hackerrank.com/challenges/weather-observation-station-3/problem
Query a list of  _CITY_  names from  **STATION**  with even  _ID_  numbers only. You may print the results in any order, but must exclude duplicates from your answer.

**Input Format**

The  **STATION**  table is described as follows:

![](https://s3.amazonaws.com/hr-challenge-images/9336/1449345840-5f0a551030-Station.jpg "Station.jpg")

where  _LAT_N_  is the northern latitude and  _LONG_W_  is the western longitude.

# Solutions
**Solution 1**:
```sql
select DISTINCT city from station where (id % 2) = 0;
```
**Solution 2**:
```sql
select DISTINCT city from station where mod(id , 2) = 0;
```
> Written with [StackEdit](https://stackedit.io/).
