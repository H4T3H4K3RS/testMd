

# **Task 1:**

Given a list of numbers `[1, 2, 3, 4, 5]`, write a Python program to find the sum of the list.

### **Solution:**

The sum of the list can be found using the built-in `sum()` function in Python.

```python
# Create a list of numbers
list_of_numbers = [1, 2, 3, 4, 5]

# Find the sum of the list
sum = sum(list_of_numbers)

# Print the result
print("The sum of the list is:", sum)
```

Output: 
```
The sum of the list is: 15
```

# **Task 2:**

Given a list of numbers `[1, 2, 3, 4, 5]`, write a Python program to find the product of the list.

### **Solution:**

The product of the list can be found by iterating over the list and multiplying each element with the result of the previous iteration.

```python
# Create a list of numbers
list_of_numbers = [1, 2, 3, 4, 5]

# Initialize the product with 1
product = 1

# Find the product of the list
for num in list_of_numbers:
    product *= num

# Print the result
print("The product of the list is:", product)
```

Output: 
```
The product of the list is: 120
```

# **Task 3:**

Write a program that prints all the elements of a list in the same order as they were inserted.

### **Solution:**

The elements of the list can be printed using a `for` loop.

```python
# Create a list
list_of_numbers = [1, 2, 3, 4, 5]

# Print all the elements of the list
for num in list_of_numbers:
    print(num)
```

Output:
```
1
2
3
4
5
```