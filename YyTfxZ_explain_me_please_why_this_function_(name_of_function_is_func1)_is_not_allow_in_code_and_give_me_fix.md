

# Solution

## Problem Description
In the given code snippet, there is a `func1` function which is not allowed in the code. The code snippet is a `while` loop which increments the value of `a` by 1 each iteration and prints the current value of `a` when it is even. 

## Solution
The `func1` function should be defined before it is used in the code. The function takes two parameters `a` and `b` and prints their values. The fixed code should look like this:

```
#!/bin/bash
a=10
c=10
b=20

func1(){
        local a=$1
        local b=$2
        echo "Function took two numbers: $a and $b"
}

while [[ $a -lt $b ]]
do
        c=$((c-a))
        func1 $a $c
        a=$((a+1))
        f=$((a%2))
        if [[ $f == 0 ]]; then
                echo "Current value of variable a is $a"
        fi
done
```