

**Solution:**

The Random Task:
Write a bash code that asks the user to enter a number and then prints the multiplication table of that number.

```bash
#!/bin/bash

#This function prints the multiplication table of the number supplied to it
function multiplicationTable() {
  number=$1

  #loop through 1 to 10
  for i in {1..10}
  do
    #calculate the result of multiplcation
    result=$(($number * $i))
    echo "$number * $i = $result"
  done
}

#ask the user to enter a number
echo "Enter a number:"

#read the user input
read number

#print the multiplication table
echo "Multiplication Table of $number:"
multiplicationTable $number
```

**Algorithm:**

1. Create a function `multiplicationTable` that takes a number as an argument
2. In the function, create a loop from `1` to `10`
3. In the loop, calculate the result of multiplication between the argument and loop variable
4. Print the result of multiplication
5. Ask the user to enter a number
6. Read the user input
7. Call the `multiplicationTable` function with the user input as an argument
8. Print the multiplication table