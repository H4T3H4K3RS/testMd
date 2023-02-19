

# **Bubble Sort Algorithm with vector<int> as Parameter**

Bubble sort is an algorithm that sorts elements of an array by repeatedly checking and swapping adjacent elements. This algorithm is simple to implement and has a time complexity of O(n<sup>2</sup>). 

## **Algorithm**

The algorithm steps are as follows:

1. Compare the first two elements of the array.
2. If the first element is greater than the second element, swap them.
3. Compare the second and third elements, then swap them if necessary.
4. Continue comparing and swapping adjacent elements until the end of the array is reached.
5. Repeat steps 1-4 until no swaps are required.

## **Code**
```cpp
// A function that sorts a vector<int> using the Bubble Sort algorithm
void bubbleSort(vector<int>& arr) {
  // Flag that will be set to false if no swaps are made in the loop
  bool swapped;

  // Loop until no swaps are made
  do {
    swapped = false;

    // Loop through the vector
    for(int i = 0; i < arr.size() - 1; i++) {
      // If the current element is greater than the next element, swap them
      if(arr[i] > arr[i + 1]) {
        swap(arr[i], arr[i + 1]);
        swapped = true;
      }
    }
  } while(swapped);
}
```