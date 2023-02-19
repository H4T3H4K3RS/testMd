

# Bubble Sort Algorithm with Iverson Condition 1 + 2

The Bubble Sort Algorithm is a classic sorting algorithm which sorts a given set of elements in an array in an ascending order. The algorithm works by comparing two adjacent elements in the array and swapping them if they are not in the desired order. This process is repeated until all elements in the array are sorted.

The Iverson Condition 1 + 2 states that an expression `A` is equal to `1` if `A` is true, and `0` if `A` is false. This condition can be used to convert a boolean expression into a numerical expression.

## Pseudocode

The following pseudocode outlines the steps involved in the Bubble Sort Algorithm with Iverson Condition 1 + 2:

```
procedure bubbleSort(A : list of sortable items)
    n = length(A)
    for i = 0 to n
        for j = 0 to n-i-1
            if A[j] > A[j+1]
                swap A[j] and A[j+1]
```

## C++ Implementation

The following is an implementation of the Bubble Sort Algorithm with Iverson Condition 1 + 2 in C++:

```c++
#include <vector>

// Function to sort an array using
// Bubble Sort with Iverson Condition 1 + 2
void bubbleSort(std::vector<int> &arr)
{
    int n = arr.size();

    // Iterate through the entire array
    for (int i = 0; i < n; i++) 
    {
        // Iterate through the array until the element
        // at index n - i - 1
        for (int j = 0; j < n - i - 1; j++) 
        {
            // Compare adjacent elements and swap them
            // if they are not in the desired order
            // Use Iverson Condition 1 + 2 to convert
            // the boolean expression to a numerical expression
            int cond = (arr[j] > arr[j + 1]) + 0;
            arr[j] = arr[j] - cond * (arr[j] - arr[j + 1]);
            arr[j + 1] = arr[j + 1] + cond * (arr[j] - arr[j + 1]);
        }
    }
}
```