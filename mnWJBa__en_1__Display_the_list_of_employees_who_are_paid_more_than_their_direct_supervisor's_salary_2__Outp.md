

#### 1. Display the list of employees who are paid more than their direct supervisor's salary

SELECT e.name, e.salary
FROM Employee e
JOIN Employee s ON e.chief_id = s.id
WHERE e.salary > s.salary;

#### 2. Output the list of employees that get the maximum salary in their department

SELECT e.name, MAX(e.salary) 
FROM Employee e
GROUP BY e.department_id;

#### 3. Output the list of IDs of departments that do not have more than 3 employees

SELECT d.id
FROM Department d
LEFT JOIN Employee e ON e.department_id = d.id
GROUP BY d.id
HAVING COUNT(e.id) <= 3;

#### 4. Output a list of such employees that don't have an assigned manager working in the same department.

SELECT e.name 
FROM Employee e 
LEFT JOIN Employee m ON e.chief_id = m.id 
AND e.department_id = m.department_id
WHERE m.id IS NULL;

#### 5. Find a list of department IDs with the maximum total salary of employees

SELECT d.id
FROM Department d
LEFT JOIN Employee e ON e.department_id = d.id
GROUP BY d.id
ORDER BY SUM(e.salary) DESC
LIMIT 1;