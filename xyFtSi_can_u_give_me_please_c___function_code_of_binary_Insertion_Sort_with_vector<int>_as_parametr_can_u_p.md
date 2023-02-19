

# Binary Insertion Sort with `vector<int>` as Parameter

This algorithm sorts an array of `N` elements in **O(N<sup>2</sup>)** time. It is a comparison based sorting algorithm and is similar to Insertion Sort, but uses binary search for the location to insert the element instead of simple linear search.

## Algorithm
1. Start from the leftmost element and consider the element to be inserted at its correct position.
2. Take the element to be inserted and use binary search to find its correct position in the sorted array.
3. Insert the element at its correct position in the sorted array.
4. Continue the same process for all the elements in the array.

## Pseudocode
```
BINARY-INSERTION-SORT(A)
  for j = 2 to A.length
    key = A[j]
    //Insert A[j] into the sorted sequence A[1..j-1]
    i = j - 1
    while i > 0 and A[i] > key
      A[i+1] = A[i]
      i = i - 1
    A[i+1] = key
```

## Implementation
```c++
// Function to perform binary insertion sort
void binaryInsertionSort(vector<int> &arr) 
{ 
    int n = arr.size(); 
    for (int i = 1; i < n; i++) 
    { 
        // Element to be inserted 
        int key = arr[i]; 
  
        // Find position to insert 
        int j = i - 1; 
  
        // Find position to insert key 
        while (j >= 0 && arr[j] > key) 
        { 
            arr[j + 1] = arr[j]; 
            j--; 
        } 
  
        // Insert the key at correct position 
        arr[j + 1] = key; 
    }
} 
```

## Time Complexity
The overall time complexity of the Binary Insertion Sort algorithm is **O(N<sup>2</sup>)**.

## Space Complexity
The Binary Insertion Sort algorithm requires **O(1)** of auxiliary space.