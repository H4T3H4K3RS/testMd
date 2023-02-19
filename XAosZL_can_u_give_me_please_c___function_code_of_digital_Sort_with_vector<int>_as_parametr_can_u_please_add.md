

# Bubble Sort Algorithm
A bubble sort algorithm is a simple sorting algorithm that repeatedly steps through the list to be sorted, compares each pair of adjacent elements and swaps them if they are in the wrong order. The algorithm, which is also known as **sinking sort**, is named for the way smaller elements **bubble** to the top of the list.

## Algorithm
The algorithm can be described in pseudocode as follows:

```
procedure BubbleSort(A : list of sortable items)
    n = length(A)
    repeat
        swapped = false
        for i = 1 to n-1 inclusive do
            if A[i-1] > A[i] then
                swap(A[i-1], A[i])
                swapped = true
            end if
        end for
    until not swapped
end procedure
```

## Implementation in C++
The following is a C++ implementation of the bubble sort algorithm:

```cpp
/*
    Bubble Sort Algorithm
    Input: Vector of integers 
    Output: Vector of sorted integers
*/

#include <iostream>
#include <vector>

void BubbleSort(std::vector<int>& arr) {
    int n = arr.size();
    bool swapped = true;
    
    // Repeat until no swaps are made
    while (swapped) {
        swapped = false;
        for (int i = 1; i < n; i++) {
            // Swap adjacent elements if they are out of order
            if (arr[i-1] > arr[i]) {
                std::swap(arr[i-1], arr[i]);
                swapped = true;
            }
        }
    }
}

int main() {
    // Unsorted vector
    std::vector<int> arr = {3, 5, 1, 6, 8, 4};

    // Perform bubble sort
    BubbleSort(arr);

    // Print sorted vector
    for (int i = 0; i < arr.size(); i++) {
        std::cout << arr[i] << " ";
    }
    std::cout << std::endl;

    return 0;
}
```