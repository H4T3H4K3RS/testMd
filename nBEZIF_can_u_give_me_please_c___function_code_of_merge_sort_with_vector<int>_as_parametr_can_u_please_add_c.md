

# __Merge Sort Algorithm with Vector<int>__

Merge sort is an efficient sorting algorithm that uses a divide-and-conquer strategy to arrange elements in a given array in increasing order. It works by repeatedly dividing the array into smaller sub-arrays and then merging them together in the proper order.

## __Algorithm Description__

1. If the input array contains fewer than two elements, then return the array.
2. Divide the array into two halves.
3. Recursively sort each half.
4. Merge the two halves together in the proper order.

## __Pseudocode__

```
MergeSort(arr[], l, r)
    if r > l
        1. Find the middle point to divide the array into two halves:  
        middle m = (l+r)/2
        2. Call mergeSort for first half:   
        Call mergeSort(arr, l, m)
        3. Call mergeSort for second half:
        Call mergeSort(arr, m+1, r)
        4. Merge the two halves sorted in step 2 and 3:
        Call merge(arr, l, m, r)
```

## __C++ Code__
```cpp
/* C++ implementation of Merge Sort */
#include <bits/stdc++.h> 
using namespace std; 

void merge(vector<int>& arr, int l, int m, int r) 
{ 
    int i, j, k; 
    int n1 = m - l + 1; 
    int n2 =  r - m; 
  
    /* create temp arrays */
    int L[n1], R[n2]; 
  
    /* Copy data to temp arrays L[] and R[] */
    for (i = 0; i < n1; i++) 
        L[i] = arr[l + i]; 
    for (j = 0; j < n2; j++) 
        R[j] = arr[m + 1+ j]; 
  
    /* Merge the temp arrays back into arr[l..r]*/
    i = 0; // Initial index of first subarray 
    j = 0; // Initial index of second subarray 
    k = l; // Initial index of merged subarray 
    while (i < n1 && j < n2) 
    { 
        if (L[i] <= R[j]) 
        { 
            arr[k] = L[i]; 
            i++; 
        } 
        else
        { 
            arr[k] = R[j]; 
            j++; 
        } 
        k++; 
    } 
  
    /* Copy the remaining elements of L[], if there 
       are any */
    while (i < n1) 
    { 
        arr[k] = L[i]; 
        i++; 
        k++; 
    } 
  
    /* Copy the remaining elements of R[], if there 
       are any */
    while (j < n2) 
    { 
        arr[k] = R[j]; 
        j++; 
        k++; 
    } 
} 
  
/* l is for left index and r is right index of the 
   sub-array of arr to be sorted */
void mergeSort(vector<int>& arr, int l, int r) 
{ 
    if (l < r) 
    { 
        int m = l+(r-l)/2; 
  
        // Sort first and second halves 
        mergeSort(arr, l, m); 
        mergeSort(arr, m+1, r); 
  
        merge(arr, l, m, r); 
    } 
} 
```