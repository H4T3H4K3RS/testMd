

# Task
Write a Bash script that reads a number from user input and prints out the factors of that number.

# Solution

```bash
#!/bin/bash

# This function takes in a number and prints out its factors
print_factors () {
  number=$1

  # Prints out the number itself as a factor
  echo "$number is its own factor"

  # Iterate from 1 to half of number
  count=1
  while [ $count -lt $(( $number / 2 )) ] 
  do
    # If number is divisible by count, it's a factor
    if [ $(( $number % $count )) -eq 0 ]
    then
      echo "$count is a factor of $number"
    fi

    # Increment count
    count=$(( $count + 1 ))
  done
}

# Read number from user input
echo -n "Enter a number: "
read number

# Validate number
if [ $number -eq 0 ]
then
  echo "Number must be a positive number!"
else
  # Call the function
  print_factors $number
fi
```