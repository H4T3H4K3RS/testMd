

# Shell Sort with Vector<int> as Parameter

Shell Sort is an algorithm which is used to sort the elements of an array or vector. It is an in-place comparison sort and is generally considered to be an improved Insertion Sort. It works by comparing elements which are far apart and then gradually reducing the gap between the elements to be compared.

## Algorithm

The following algorithm is used for Shell Sort:

1. Start with a gap value `gap`;
2. Compare elements `A[i]` and `A[i + gap]`;
3. Swap `A[i]` and `A[i + gap]` if `A[i] > A[i + gap]`;
4. Set `gap = gap/2`;
5. Repeat step 2 for the elements `A[i]` and `A[i + gap]` until `gap = 1`;
6. Repeat steps 2, 3, 4 and 5 until all elements are sorted.

## Pseudocode

```
function shellSort(arr[]) 
{
    // Start with a big gap, then reduce the gap 
    for (gap = arr.length/2; gap > 0; gap /= 2) 
    { 
        // Do a gapped insertion sort for this gap size. 
        // The first gap elements arr[0..gap-1] are already in gapped order 
        // keep adding one more element until the entire array is gap sorted 
        for (int i = gap; i < arr.length; i += 1) 
        { 
            // add arr[i] to the elements that have been gap sorted 
            // save arr[i] in temp and make a hole at position i 
            int temp = arr[i]; 
  
            // shift earlier gap-sorted elements up until the correct location for arr[i] is found 
            int j;             
            for (j = i; j >= gap && arr[j - gap] > temp; j -= gap) 
                arr[j] = arr[j - gap]; 
  
            // put temp (the original arr[i]) in its correct location 
            arr[j] = temp; 
        } 
    } 
} 
```

## C++ Code

```cpp
// C++ code for Shell Sort
// function to sort vector<int> 
void shellSort(vector<int> &arr) 
{ 
    // Start with a big gap, then reduce the gap 
    for (int gap = arr.size()/2; gap > 0; gap /= 2) 
    { 
        // Do a gapped insertion sort for this gap size. 
        // The first gap elements arr[0..gap-1] are already in gapped order 
        // keep adding one more element until the entire array is gap sorted 
        for (int i = gap; i < arr.size(); i += 1) 
        { 
            // add arr[i] to the elements that have been gap sorted 
            // save arr[i] in temp and make a hole at position i 
            int temp = arr[i]; 
  
            // shift earlier gap-sorted elements up until the correct location for arr[i] is found 
            int j;             
            for (j = i; j >= gap && arr[j - gap] > temp; j -= gap) 
                arr[j] = arr[j - gap]; 
  
            // put temp (the original arr[i]) in its correct location 
            arr[j] = temp; 
        } 
    } 
} 
```

## Complexity

The time complexity of Shell Sort depends on the gap sequence used. For worst case, the time complexity of Shell Sort is:

$$
\mathcal{O}(n^2)
$$

For best case, the time complexity of Shell Sort is:

$$
\mathcal{O}(n)
$$

The space complexity of Shell Sort is:

$$
\mathcal{O}(1)
$$