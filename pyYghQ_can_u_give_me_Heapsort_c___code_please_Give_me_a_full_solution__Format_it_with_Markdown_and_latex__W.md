

## Heapsort 

Heapsort is an in-place sorting algorithm that sorts an array of comparable elements into a **heap** data structure in **O(n)** time, and then **removes** the maximum element from the heap and places it at the end of the array, reducing the size of the heap by one. Heapsort is an efficient sorting algorithm with **average** and **worst-case** complexities of **O(n log n)**, making it **more efficient** than **quicksort** and **mergesort**.

### Steps of Heapsort 

Heapsort is composed of two steps: 

1. Building a heap out of the data
2. Removing the largest item and replacing it with the next item in the heap (repeated until the heap is empty)

### Pseudocode

The following is a pseudocode implementation of Heapsort: 

```
Heapsort(A)
    BuildHeap(A)
    for i = n downto 2
        swap A[1] with A[i]
        n = n - 1
        Heapify(A, 1)   

BuildHeap(A)
    n = length[A]
    for i = floor(n/2) downto 1
        Heapify(A, i)

Heapify(A, i)
    l = left(i)
    r = right(i)
    if l <= n and A[l] > A[i]
        largest = l
    else 
        largest = i
    if r <= n and A[r] > A[largest]
        largest = r
    if largest != i
        swap A[i] with A[largest]
        Heapify(A, largest)
```

### Algorithm

Heapsort works by first converting an array into a **max-heap**, a data structure that can be sorted in-place. This is done by starting from the **midpoint** of the array and **heapifying** each element downwards, until the entire array is a heap. After this is done, the maximum element is extracted from the heap and placed at the end of the array. This process is repeated until the heap is empty.

### Time Complexity

The time complexity of Heapsort is **O(n log n)**. This is because, while building the heap is an **O(n)** operation, the Heapify operation is done **log n** times for each element in the array, leading to a total complexity of **O(n log n)**.

### Space Complexity

The space complexity of Heapsort is **O(1)**, as the algorithm works in-place, meaning that no extra space is required.