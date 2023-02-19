

# Heap Sort using Vector<int>
Heap sort is an in-place sorting algorithm with an average time complexity of **O(n log n)**. It is a comparison based sorting algorithm which uses a data structure called heap. Heaps are binary trees for which every parent node has a value less than or equal to any of its children. 

## Algorithm
Given a collection of elements, the heap sort algorithm involves the following steps:
1. Create a heap from the elements.
2. Remove the top element from the heap.
3. Replace it with the last element of the heap.
4. Repeat steps 2 and 3 until the heap is empty.

## Code
```cpp
// Heap sort function
void heapSort(vector<int>& arr) 
{ 
    int n = arr.size(); 
  
    // Create a heap using the given array 
    for (int i = n / 2 - 1; i >= 0; i--) 
        heapify(arr, n, i); 
  
    // Extract elements one by one 
    for (int i = n - 1; i >= 0; i--) 
    { 
        // Move current root to end 
        swap(arr[0], arr[i]); 
  
        // call max heapify on the reduced heap 
        heapify(arr, i, 0); 
    } 
} 

// To heapify a subtree rooted with node i which is 
// an index in arr[]. n is size of heap 
void heapify(vector<int>& arr, int n, int i) 
{ 
    int largest = i; // Initialize largest as root 
    int l = 2 * i + 1; // left = 2*i + 1 
    int r = 2 * i + 2; // right = 2*i + 2 
  
    // If left child is larger than root 
    if (l < n && arr[l] > arr[largest]) 
        largest = l; 
  
    // If right child is larger than largest so far 
    if (r < n && arr[r] > arr[largest]) 
        largest = r; 
  
    // If largest is not root 
    if (largest != i) 
    { 
        swap(arr[i], arr[largest]); 
  
        // Recursively heapify the affected sub-tree 
        heapify(arr, n, largest); 
    } 
} 
```