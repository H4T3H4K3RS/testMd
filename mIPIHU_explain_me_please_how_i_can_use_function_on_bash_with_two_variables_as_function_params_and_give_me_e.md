

# Solution 

We will use a function in Bash to demonstrate how to use two variables as function parameters.

## Definition of Function 
A function is a block of code that performs a specific task and returns a value. It can take multiple parameters as input, and those parameters can be used to control the behavior of the function.

## Syntax 
The syntax for defining a function in Bash is as follows:

```
funcName () {
  # code here
}
```

Where `funcName` is the name of the function, and the `# code here` is the code that will be executed when the function is called.

## Example

Let's say we want to define a function called `add` that takes two numbers as parameters and returns the sum. The function definition would look like this:

```
add () {
  sum=$(( $1 + $2 ))
  echo $sum
}
```

Here, `$1` and `$2` are the parameters that we pass to the function. We use them to calculate the sum, which is then stored in the variable `sum`. Finally, we `echo` the value of `sum`.

## Usage

Now that we have defined the `add` function, we can use it anywhere in our Bash script. To call the function, we use the following syntax:

```
add <argument1> <argument2>
```

Where `<argument1>` and `<argument2>` are the values that we want to pass to the function. For example, if we want to add the numbers 5 and 10, we can call the `add` function like this:

```
add 5 10
```

This will output the value `15`, which is the sum of 5 and 10.