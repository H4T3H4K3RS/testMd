

# Bubble Sort Algorithm

Bubble Sort is a simple sorting algorithm that repeatedly steps through the list to be sorted, compares each pair of adjacent items and swaps them if they are in the wrong order. The pass through the list is repeated until no swaps are needed, which indicates that the list is sorted.

The following code implements Bubble Sort algorithm:

```
void bubbleSortA1(vector<int> &arr) {
    int n = arr.size();
    for (int i = 0; i < n - 1; i++) {
        bool swapped = false;
        for (int j = 0; j < n - i - 1; j++)
            if (arr[j] > arr[j + 1]) {
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
                swapped = true;
            }
        if (!swapped) {
            break;
        }
    }
}
```

## Algorithm Complexity

The time complexity of Bubble Sort algorithm is $$O(n^2)$$, where $$n$$ is the number of elements in the array. This is because for each element in the array, it needs to compare with every other element in the array.

The space complexity of Bubble Sort algorithm is $$O(1)$$, as it only requires a single auxiliary variable to store the data while swapping.