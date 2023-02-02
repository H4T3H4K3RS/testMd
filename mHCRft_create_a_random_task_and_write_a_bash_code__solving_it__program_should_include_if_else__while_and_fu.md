

# Generating Random Numbers

## Overview

This bash script will generate random numbers between 1 and 10 and check if the generated numbers are even or odd.

## Algorithm

1. Declare a function to generate random numbers and a variable to store the generated numbers.
```bash
generate_random_number() {
  # Generate random number between 1 and 10
  local random_number=$(( ( RANDOM % 10 )  + 1 ))
}
```
2. Use a while loop to call the random number generator function and store the generated numbers in the variable.
```bash
# Declare variable to store random numbers
random_numbers=()

# Generate random numbers between 1 and 10
while [[ ${#random_numbers[@]} -lt 10 ]]
do
  generate_random_number
  random_numbers+=($random_number)
done
```
3. Use an if-else statement to check if each generated number is even or odd.
```bash
# Check if the generated numbers are even or odd
for num in ${random_numbers[@]}
do 
  # Check if number is even
  if [[ $((num % 2)) -eq 0 ]]
  then
    echo "$num is even"
  else
    echo "$num is odd"
  fi
done
```

## Final Code

```bash
#!/bin/bash

# Declare function to generate random numbers
generate_random_number() {
  # Generate random number between 1 and 10
  local random_number=$(( ( RANDOM % 10 )  + 1 ))
}

# Declare variable to store random numbers
random_numbers=()

# Generate random numbers between 1 and 10
while [[ ${#random_numbers[@]} -lt 10 ]]
do
  generate_random_number
  random_numbers+=($random_number)
done

# Check if the generated numbers are even or odd
for num in ${random_numbers[@]}
do 
  # Check if number is even
  if [[ $((num % 2)) -eq 0 ]]
  then
    echo "$num is even"
  else
    echo "$num is odd"
  fi
done
```