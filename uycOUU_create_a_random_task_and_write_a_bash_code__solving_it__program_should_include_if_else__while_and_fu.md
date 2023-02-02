

# **Task:** Generate a random number between 0 and 100 and print the result  

## Solution

```bash
#!/bin/bash

# Generate a random number between 0 and 100
# and print the result

# Define a function to generate a random number
function random_gen {
  # Generate a random number between 0 and 1
  random_num=$(echo "scale=2; $RANDOM/32767" | bc -l)
  # Multiply by 100 to get a number between 0 and 100
  result=$(echo "scale=2; $random_num*100" | bc -l)
  # Print the result
  echo "$result"
}

# While loop to check the result
while [ true ]
do
  # Call the function
  result=$(random_gen)
  # Check if result is between 0 and 100
  if [[ $(echo "scale=2; $result > 0" | bc -l) -eq 1 &&  $(echo "scale=2; $result < 100" | bc -l) -eq 1 ]]
  then
    # Print the result if it is between 0 and 100
    echo "Random number is $result"
    break
  fi
done

```