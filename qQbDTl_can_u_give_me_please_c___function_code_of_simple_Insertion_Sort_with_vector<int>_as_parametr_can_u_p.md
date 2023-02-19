

# Insertion Sort with Vector<int> as Parameter

Insertion sort is an in-place sorting algorithm which is efficient for small data sets. It works by building the final sorted array one item at a time. It is a comparison based sorting algorithm and has a time complexity of **O(n<sup>2</sup>)**.

## Algorithm

1. Start by picking the second element in the array.
2. Compare the second element with the one before it and swap if necessary.
3. Continue to the next element and if it is in the incorrect order, iterate through the sorted portion (i.e. the left side) to place the element in the correct place.
4. Repeat until the array is sorted.

## C++ Code

```c++
// Insertion Sort with Vector<int> as Parameter
void insertionSort(vector<int> &arr) 
{ 
    int n = arr.size(); 
    for (int i = 1; i < n; i++) 
    { 
        int key = arr[i]; 
        int j = i - 1; 
  
        while (j >= 0 && arr[j] > key) 
        { 
            arr[j + 1] = arr[j]; 
            j = j - 1; 
        } 
        arr[j + 1] = key; 
    } 
}
```