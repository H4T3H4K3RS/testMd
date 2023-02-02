

# **Random Task:** Generate a Random Password 

The following bash code will generate a random password with 8 characters. The characters will be either an uppercase letter, lowercase letter, or a number.

**Solution:**

```bash
#!/bin/bash

# This function generates a random character
function randomCharacter(){
    # Generate a number from 0 to 2
    randomNumber=$(( $RANDOM % 3 ))
        
    # If the number is 0, return an uppercase letter
    if [[ $randomNumber == 0 ]]; then
        randomCharacter=$(echo $(( $RANDOM % 26 + 65 )) | awk '{printf "%c",$0}')
    # If the number is 1, return a lowercase letter
    elif [[ $randomNumber == 1 ]]; then
        randomCharacter=$(echo $(( $RANDOM % 26 + 97 )) | awk '{printf "%c",$0}')
    # If the number is 2, return a number
    else
        randomCharacter=$(echo $(( $RANDOM % 10 + 48 )) | awk '{printf "%c",$0}')
    fi
}

# Initialize the password variable
password=''

# Generate 8 random characters and append to the password variable
while [[ ${#password} -lt 8 ]]; do
    randomCharacter
    password="$password$randomCharacter"
done

# Print the randomly generated password
echo $password
```