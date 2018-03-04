## Employee Salaries
Source: https://www.hackerrank.com/challenges/salary-of-employees/problem
Write a query that prints a list of employee names (i.e.: the  _name_  attribute) for employees in  **Employee**  having a salary greater than  per month who have been employees for less than  months. Sort your result by ascending  _employee_id_.

**Input Format**

The  **Employee**  table containing employee data for a company is described as follows:

![](https://s3.amazonaws.com/hr-challenge-images/19629/1458557872-4396838885-ScreenShot2016-03-21at4.27.13PM.png)

where  _employee_id_  is an employee's ID number,  _name_  is their name,  _months_  is the total number of months they've been working for the company, and  _salary_  is the their monthly salary.

**Sample Input**

![](https://s3.amazonaws.com/hr-challenge-images/19630/1458558612-af3da3ceb7-ScreenShot2016-03-21at4.32.59PM.png)

**Sample Output**

```
Angela
Michael
Todd
Joe

```

**Explanation**

_Angela_  has been an employee for  month and earns  per month.

_Michael_  has been an employee for  months and earns  per month.

_Todd_  has been an employee for  months and earns  per month.

_Joe_  has been an employee for  months and earns  per month.

We order our output by ascending  _employee_id_.


---
# Solution
```sql
SELECT name
FROM Employee 
WHERE salary > 2000 AND months < 10
```
