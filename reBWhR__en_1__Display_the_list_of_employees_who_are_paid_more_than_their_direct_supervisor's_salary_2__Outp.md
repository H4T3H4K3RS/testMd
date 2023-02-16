

**Solution:**

1. Display the list of employees who are paid more than their direct supervisor's salary

```SQL
SELECT e.ID, e.Name, e.Salary
FROM Employee e
INNER JOIN Employee e2 ON e2.ID = e.Chief_ID
WHERE e.Salary > e2.Salary;
```

2. Output the list of employees that get the maximum salary in their department

```SQL
SELECT e.ID, e.Name, e.Salary
FROM Employee e
INNER JOIN (
    SELECT Department_ID, MAX(Salary) AS MaxSalary
    FROM Employee
    GROUP BY Department_ID
) AS MaxSalaries ON MaxSalaries.Department_ID = e.Department_ID AND MaxSalaries.MaxSalary = e.Salary;
```

3. Output the list of IDs of departments that do not have more than 3 employees

```SQL
SELECT Department_ID
FROM Employee
GROUP BY Department_ID
HAVING COUNT(*) <= 3;
```

4. Output a list of such employees that don't have an assigned manager working in the same department.

```SQL
SELECT e.ID, e.Name
FROM Employee e
WHERE e.Chief_ID IS NULL
AND NOT EXISTS (
    SELECT *
    FROM Employee e2
    WHERE e2.Department_ID = e.Department_ID
    AND e2.Chief_ID IS NULL
);
```

5. Find a list of department IDs with the maximum total salary of employees

```SQL
SELECT Department_ID, SUM(Salary) AS TotalSalary
FROM Employee
GROUP BY Department_ID
HAVING SUM(Salary) = (
    SELECT MAX(TotalSalary)
    FROM (
        SELECT Department_ID, SUM(Salary) AS TotalSalary
        FROM Employee
        GROUP BY Department_ID
    )
);
```