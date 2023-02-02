

# Function on Bash with Two Variables

In Bash, it is possible to create and use functions with two variables. This can be done using the following syntax:

```bash
function <function_name>() {
  # Function code goes here
  <variable1>=<value1>
  <variable2>=<value2>
  # More code
}
```

where `<function_name>` is the name of the function, `<variable1>` and `<variable2>` are the two variables, and `<value1>` and `<value2>` are the values assigned to each variable.

## Example 1

Let's say we want to create a function `greet()` that prints out a greeting message using two variables: `name` and `age`. We can do this as follows:

```bash
function greet() {
  name=John
  age=25
  echo "Hello, my name is $name and I am $age years old."
}
```

Now, when we call the `greet()` function, the following will be printed:

```
Hello, my name is John and I am 25 years old.
```

## Example 2

Let's create a function `calculate()` that calculates the sum of two numbers using two variables: `x` and `y`. We can do this as follows:

```bash
function calculate() {
  x=3
  y=5
  sum=$(( x + y ))
  echo "The sum of $x and $y is $sum."
}
```

Now, when we call the `calculate()` function, the following will be printed:

```
The sum of 3 and 5 is 8.
```

Using functions with two variables in Bash is a useful way to quickly and easily execute code that requires multiple variables.