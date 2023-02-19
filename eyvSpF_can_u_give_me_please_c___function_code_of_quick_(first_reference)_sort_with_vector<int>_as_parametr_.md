

# Quick Sort with Vector<int> as Parameter

Quick Sort is an efficient sorting algorithm which follows the divide-and-conquer approach. It works by partitioning the array into two sub-arrays: the sub-array of elements less than the pivot element and the sub-array of elements greater than the pivot element. The algorithm then recursively sorts the two sub-arrays.

**Algorithm**

1. Select a pivot element `p` from the array
2. Partition the array into two sub-arrays `A<sub>1</sub>` and `A<sub>2</sub>`
   - `A<sub>1</sub>` contains all elements less than `p`
   - `A<sub>2</sub>` contains all elements greater than `p`
3. Recursively sort the two sub-arrays using Quick Sort

**Pseudocode**

```
QuickSort(A, low, high)
1 if (low < high)
2   p := Partition(A, low, high)
3   QuickSort(A, low, p - 1)
4   QuickSort(A, p + 1, high)

Partition(A, low, high)
1 pivot := A[high]
2 i := low
3 for j := low to high - 1
4   if (A[j] <= pivot)
5     swap A[i] with A[j]
6     i := i + 1
7 swap A[i] with A[high]
8 return i
```

**C++ Code**
```cpp
// Quick Sort with Vector<int> as Parameter
#include <vector>

int Partition(std::vector<int>& A, int low, int high)
{
    int pivot = A[high];
    int i = low;
    for (int j = low; j < high; j++)
    {
        if (A[j] <= pivot)
        {
            std::swap(A[i], A[j]);
            i++;
        }
    }
    std::swap(A[i], A[high]);
    return i;
}

void QuickSort(std::vector<int>& A, int low, int high)
{
    if (low < high)
    {
        int p = Partition(A, low, high);
        QuickSort(A, low, p - 1);
        QuickSort(A, p + 1, high);
    }
}
```