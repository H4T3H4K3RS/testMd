

# Binary Insertion Sort with Vector<int> as Parameter 
This function uses Binary Insertion Sort to sort a vector of integers.

## Algorithm
1. Begin with a sorted sublist in the lower positions of the list.
2. Pick element from the unsorted sublist and insert it in the correct position of the sorted sublist.

## Pseudo Code
```
BinaryInsertionSort(vector<int> arr)
  // Set left and right to the first and last element of the vector respectively
  left = 0
  right = arr.size() - 1
  
  // Iterate over all elements in the vector
  for i = 1 to right do
      x = arr[i]
      left = 0
      right = i - 1
 
      // Find the correct position of the element in the sorted sublist
      while (left <= right) do
          mid = (left + right) / 2
          if (arr[mid] > x) then
              right = mid - 1
          else
              left = mid + 1
      end while
 
      // Shift all elements from left to right
      j = i - 1
      while (j >= left) do
          arr[j+1] = arr[j]
          j = j - 1
      end while
 
      // Insert the element in the correct position
      arr[left] = x
  end for
end BinaryInsertionSort
```

## Time Complexity
The time complexity of Binary Insertion Sort is $$\mathcal{O}(n^2)$$.