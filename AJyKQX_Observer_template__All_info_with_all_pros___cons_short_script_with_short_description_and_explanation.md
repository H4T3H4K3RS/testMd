

# _Template Method Design Pattern_
The Template Method design pattern is a behavioral design pattern that defines the program skeleton of an algorithm in a method, called the template method, which defers some steps to subclasses. It lets one redefine certain steps of an algorithm without changing the algorithm's structure.

## Pros
- Allows subclasses to redefine certain steps of an algorithm without changing the algorithm's structure
- Makes code easier to read and maintain
- Improves code reusability, since the same template can be used for different algorithms

## Cons
- Adds complexity, since the template method and its subclasses must be designed and maintained together
- Can lead to code bloat if the template method is overused
- Can lead to code duplication if the same steps are repeated in multiple subclasses

## Use Cases
The Template Method pattern is most useful when there are multiple algorithms that are similar but differ in certain steps. This pattern can help avoid code duplication and make the code easier to read and maintain.

## Example
Let's consider a situation where we need to implement two algorithms for sorting an array, one using insertion sort and the other using selection sort.

We could define an abstract class with a template method that contains the basic structure of the algorithm, such as looping over the array and swapping elements. The template method would then defer the actual sorting steps to subclasses, which would implement the sorting algorithms. This way, we could reuse the same template for both sorting algorithms, and only have to implement the sorting steps in the subclasses.

## Pseudocode
```
abstract class SortAlgorithm 
  templateMethod()
    loop over the array 
    swap elements 
    call abstract method sortSteps()
  
  abstract method sortSteps()
  
class InsertionSort extends SortAlgorithm 
  sortSteps() 
    use insertion sort algorithm 
    
class SelectionSort extends SortAlgorithm 
  sortSteps() 
    use selection sort algorithm
```