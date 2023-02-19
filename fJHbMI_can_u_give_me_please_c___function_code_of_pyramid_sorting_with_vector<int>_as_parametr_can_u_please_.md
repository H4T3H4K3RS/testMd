

# Pyramid Sorting with vector<int>

Pyramid sorting is an efficient sorting algorithm used to sort an array in an ascending order. It is a stable sorting algorithm, meaning that it preserves the relative order of equal elements. The algorithm works by repeatedly dividing the array into two halves and then sorting the two halves. The sorting is done using a pyramid-like structure.

## Algorithm

Given an array of integers, the algorithm works as follows:

1. Divide the array into two halves.
2. Sort each half using a standard sorting algorithm.
3. Merge the two sorted halves into a single array using the pyramid structure.

The pyramid structure is a two-dimensional array with the following properties:

- The first row contains the elements from the first half of the original array.
- The second row contains the elements from the second half of the original array.
- The third row contains the elements from the first and second rows combined, sorted in ascending order.
- The fourth row contains the elements from the third row combined, sorted in ascending order.
- The fifth row contains the elements from the fourth row combined, sorted in ascending order.

This process is repeated until a single sorted array is obtained.

## Pseudocode

The following pseudocode describes the algorithm in more detail:

```
function pyramidSort(array):
    // Divide the array into two halves
    left = array[0..n/2]
    right = array[n/2+1..n]

    // Sort each half using a standard sorting algorithm
    left = sort(left)
    right = sort(right)

    // Merge the two sorted halves into a single array
    result = merge(left, right)

    // Repeat the process until a single sorted array is obtained
    while result.length > 1:
        // Divide the result into two halves
        left = result[0..n/2]
        right = result[n/2+1..n]

        // Merge the two sorted halves into a single array
        result = merge(left, right)

return result

// Merge two sorted arrays into a single array
function merge(left, right):
    // Initialize result array
    result = []

    // Iterate over each element in the left and right arrays
    while left.length > 0 and right.length > 0:
        // Compare the first elements of the left and right arrays
        if left[0] <= right[0]:
            // Add the element from the left array to the result array
            result.append(left[0])
            // Remove the element from the left array
            left.remove(left[0])
        else:
            // Add the element from the right array to the result array
            result.append(right[0])
            // Remove the element from the right array
            right.remove(right[0])

    // Add the remaining elements from the left array to the result array
    for element in left:
        result.append(element)

    // Add the remaining elements from the right array to the result array
    for element in right:
        result.append(element)

    return result
```

## C++ Implementation

The following is a C++ implementation of the pseudocode described above:

```cpp
#include <vector>

std::vector<int> pyramidSort(std::vector<int> array) {
    // Divide the array into two halves
    std::vector<int> left(array.begin(), array.begin() + array.size() / 2);
    std::vector<int> right(array.begin() + array.size() / 2, array.end());

    // Sort each half using a standard sorting algorithm
    std::sort(left.begin(), left.end());
    std::sort(right.begin(), right.end());

    // Merge the two sorted halves into a single array
    std::vector<int> result = merge(left, right);

    // Repeat the process until a single sorted array is obtained
    while (result.size() > 1) {
        // Divide the result into two halves
        left.assign(result.begin(), result.begin() + result.size() / 2);
        right.assign(result.begin() + result.size() / 2, result.end());

        // Merge the two sorted halves into a single array
        result = merge(left, right);
    }

    return result;
}

// Merge two sorted arrays into a single array
std::vector<int> merge(std::vector<int> left, std::vector<int> right) {
    // Initialize result array
    std::vector<int> result;

    // Iterate over each element in the left and right arrays
    while (left.size() > 0 && right.size() > 0) {
        // Compare the first elements of the left and right arrays
        if (left[0] <= right[0]) {
            // Add the element from the left array to the result array
            result.push_back(left[0]);
            // Remove the element from the left array
            left.erase(left.begin());
        } else {
            // Add the element from the right array to the result array
            result.push_back(right[0]);
            // Remove the element from the right array
            right.erase(right.begin());
        }
    }

    // Add the remaining elements from the left array to the result array
    for (int element : left) {
        result.push_back(element);
    }

    // Add the remaining elements from the right array to the result array
    for (int element : right) {
        result.push_back(element);
    }

    return result;
}
```