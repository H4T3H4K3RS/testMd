

# **Selection Sort Algorithm with vector<int> as parameter**

Selection sort is an algorithm that sorts an array by repeatedly finding the minimum element (considering ascending order) from unsorted part and putting it at the beginning. The algorithm maintains two subarrays in a given array.

1. The subarray which is already sorted.
2. Remaining subarray which is unsorted.

In every iteration of selection sort, the minimum element (considering ascending order) from the unsorted subarray is picked and moved to the sorted subarray.

<div align="center">
\begin{equation*}
Time\ Complexity\ of\ Selection\ Sort\ =\ O(n^2)
\end{equation*}
</div>

## **C++ Implementation of Selection Sort with vector<int> as parameter**

```cpp
// C++ program for implementation of Selection Sort
#include <bits/stdc++.h>
using namespace std;

// Function to implement selection sort algorithm
void selectionSort(vector<int> &arr, int n)
{
    int i, j, min_idx;
 
    // One by one move boundary of unsorted subarray
    for (i = 0; i < n-1; i++)
    {
        // Find the minimum element in unsorted array
        min_idx = i;
        for (j = i+1; j < n; j++)
          if (arr[j] < arr[min_idx])
            min_idx = j;
 
        // Swap the found minimum element with the first element
        swap(arr[min_idx], arr[i]);
    }
}

// Print the array
void printArray(vector<int> arr, int size)
{
    int i;
    for (i=0; i < size; i++)
        cout << arr[i] << " ";
    cout << endl;
}
 
// Driver program to test above functions
int main()
{
    vector<int> arr = {64, 25, 12, 22, 11};
    int n = arr.size();
    selectionSort(arr, n);
    cout << "Sorted array: \n";
    printArray(arr, n);
    return 0;
}
```

**Output:**

Sorted array: 
11 12 22 25 64