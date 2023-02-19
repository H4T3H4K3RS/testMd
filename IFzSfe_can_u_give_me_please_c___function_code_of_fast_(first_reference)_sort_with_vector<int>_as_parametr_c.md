

# Fast Sort Algorithm

A fast sort algorithm is a sorting algorithm that is able to sort a given array in an efficient and optimal manner. This algorithm is usually implemented using a divide-and-conquer approach, where the array is divided into two sub-arrays and the sub-arrays are then sorted recursively.

## Algorithm

The following is a pseudocode for the fast sort algorithm.

```
FastSort(array A, int low, int high):
    if low < high:
        // Partition the array
        int pivotIndex = Partition(A, low, high)
        
        // Sort the sub-arrays recursively
        FastSort(A, low, pivotIndex - 1)
        FastSort(A, pivotIndex + 1, high)

Partition(array A, int low, int high):
    // Select the pivot element
    int pivot = A[high]
    int i = low - 1

    // Rearrange the elements around the pivot
    for j = low to high:
        if A[j] <= pivot:
            i = i + 1
            swap(A[i], A[j])

    // Swap the pivot element with the element at index i
    swap(A[i + 1], A[high])
    
    // Return the index of the pivot element
    return i + 1
```

## C++ Implementation

The following is a C++ implementation of the fast sort algorithm.

```cpp
// Function to partition the array
int Partition(std::vector<int>& A, int low, int high)
{
    // Select the pivot element
    int pivot = A[high];
    int i = low - 1;

    // Rearrange the elements around the pivot
    for (int j = low; j <= high; j++)
    {
        if (A[j] <= pivot)
        {
            i = i + 1;
            std::swap(A[i], A[j]);
        }
    }

    // Swap the pivot element with the element at index i
    std::swap(A[i + 1], A[high]);

    // Return the index of the pivot element
    return i + 1;
}

// Fast Sort Algorithm
void FastSort(std::vector<int>& A, int low, int high)
{
    if (low < high)
    {
        // Partition the array
        int pivotIndex = Partition(A, low, high);

        // Sort the sub-arrays recursively
        FastSort(A, low, pivotIndex - 1);
        FastSort(A, pivotIndex + 1, high);
    }
}
```