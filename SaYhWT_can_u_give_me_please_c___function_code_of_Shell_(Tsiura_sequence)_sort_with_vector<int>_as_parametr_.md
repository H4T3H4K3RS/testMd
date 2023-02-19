

# Shell Sort with Vector<int> as Parameter
Shell Sort is a type of sorting algorithm that is based on the insertion sort algorithm. It works by comparing elements that are a certain distance apart, called the gap, and then comparing them. It then rearranges the elements accordingly.

## Algorithm
The Shell Sort algorithm works by comparing elements that are a certain distance apart and then rearranging them accordingly. The gap size can be varied to improve the performance of the algorithm.

1. Set the gap size to half the size of the array.
2. Compare elements that are gap size apart.
3. Rearrange the elements accordingly.
4. If the gap size is greater than 1, divide the gap size by 2 and repeat step 2.
5. Once the gap size is 1, the array is sorted.

## Implementation
The following is an implementation of the Shell Sort algorithm using a vector of integers as the parameter.

```cpp
void shellSort(vector<int>& arr) 
{ 
    // Start with a big gap, then reduce the gap 
    for (int gap = arr.size()/2; gap > 0; gap /= 2) 
    { 
        // Do a gapped insertion sort for this gap size. 
        // The first gap elements a[0..gap-1] are already in gapped order 
        // keep adding one more element until the entire array is 
        // gap sorted 
        for (int i = gap; i < arr.size(); i += 1) 
        { 
            // add a[i] to the elements that have been gap sorted 
            // save a[i] in temp and make a hole at position i 
            int temp = arr[i]; 
  
            // shift earlier gap-sorted elements up until the correct 
            // location for a[i] is found 
            int j;             
            for (j = i; j >= gap && arr[j - gap] > temp; j -= gap) 
                arr[j] = arr[j - gap]; 
              
            //  put temp (the original a[i]) in its correct location 
            arr[j] = temp; 
        } 
    } 
} 
```

## Complexity
The time complexity of Shell Sort is **O(n<sup>2</sup>)** in the worst case and it is **O(nlog<sub>2</sub>n)** in the best case. The space complexity of Shell Sort is **O(1)**.