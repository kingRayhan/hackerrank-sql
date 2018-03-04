## Higher Than 75 Marks
Query the  _Name_  of any student in  **STUDENTS**  who scored higher than  _Marks_. Order your output by the  _last three characters_  of each name. If two or more students both have names ending in the same last three characters (i.e.: Bobby, Robby, etc.), secondary sort them by ascending  _ID_.

**Input Format**

The  **STUDENTS**  table is described as follows:
![](https://s3.amazonaws.com/hr-challenge-images/12896/1443815243-94b941f556-1.png)

The  _Name_  column only contains uppercase (`A`-`Z`) and lowercase (`a`-`z`) letters.

**Sample Input**

![](https://s3.amazonaws.com/hr-challenge-images/12896/1443815209-cf4b260993-2.png)

**Sample Output**

```
Ashley
Julia
Belvet

```

**Explanation**

Only Ashley, Julia, and Belvet have  _Marks_  >  . If you look at the last three characters of each of their names, there are no duplicates and 'ley' < 'lia' < 'vet'.


---

### Solution
```sql
SELECT Name FROM STUDENTS
WHERE Marks > 75
ORDER BY RIGHT(Name, 3), ID;
```
