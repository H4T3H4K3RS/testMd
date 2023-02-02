

# **Task:** Write a Bash script to calculate the sum of the numbers from 1 to 10

```bash 
#!/bin/bash

# Variable to store the sum
sum=0

# Function to calculate the sum
calculateSum() {
	for i in {1..10}
	do
		((sum+=i))
	done	
}

# Calling the function
calculateSum

# Print the result
echo "The sum of numbers from 1 to 10 is: $sum"
```

**Solution:**

The Bash script to calculate the sum of the numbers from 1 to 10 is as follows: 

```bash
#!/bin/bash

# Variable to store the sum
sum=0

# Function to calculate the sum
calculateSum() {
	for i in {1..10}
	do
		((sum+=i))
	done	
}

# Calling the function
calculateSum

# Print the result
echo "The sum of numbers from 1 to 10 is: $sum"
```

The algorithm used in this script is as follows: 

1. Initialize a variable `sum` to store the sum of the numbers from 1 to 10
2. Create a function `calculateSum` to calculate the sum of the numbers from 1 to 10
   1. For each number in the range of 1 to 10
   2. Add the number to the `sum` variable
3. Call the `calculateSum` function
4. Print the `sum` variable, which contains the sum of the numbers from 1 to 10