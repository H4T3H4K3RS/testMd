

# Solution

## 1. Display the list of employees who are paid more than their direct supervisor's salary

SELECT e.name 
FROM Employee e 
JOIN Employee c 
ON e.chief_id = c.id 
WHERE e.salary > c.salary;

## 2. Output the list of employees that get the maximum salary in their department

SELECT e.name 
FROM Employee e 
JOIN (SELECT department_id, MAX(salary) as max_salary 
	FROM Employee 
	GROUP BY department_id) max_sal
ON e.department_id = max_sal.department_id
AND e.salary = max_sal.max_salary;
 
## 3. Output the list of IDs of departments that do not have more than 3 employees

SELECT id 
FROM Department 
WHERE id NOT IN (SELECT department_id 
				  FROM Employee 
				  GROUP BY department_id 
				  HAVING COUNT(*) > 3);

## 4. Output a list of such employees that don't have an assigned manager working in the same department.

SELECT e.name 
FROM Employee e 
LEFT JOIN Employee c 
ON e.chief_id = c.id 
AND e.department_id = c.department_id 
WHERE c.id IS NULL;

## 5. Find a list of department IDs with the maximum total salary of employees

SELECT department_id, SUM(salary) as total_salary 
FROM Employee 
GROUP BY department_id 
ORDER BY total_salary DESC 
LIMIT 1;