

# Bubble Sort Algorithm with Iverson condition 1

Bubble sort is a comparison-based sorting algorithm. It works by repeatedly swapping the adjacent elements if they are in the wrong order.

## Iverson condition 1
The Iverson condition is a formalised way to express a boolean value as a numerical value. It uses a 0-1 notation where 0 is False and 1 is True.

## Code

```cpp
vector<int> bubbleSort(vector<int> arr)  
{  
    int n = arr.size();  
    for (int i = 0; i < n-1; i++)      
        for (int j = 0; j < n-i-1; j++)  
            if (arr[j] > arr[j+1])  
            {
                int temp = arr[j];
                arr[j] = arr[j+1];
                arr[j+1] = temp;
            }

    // Iverson Condition
    int sorted = (arr == vector<int>(arr.begin(), arr.end())) ? 1 : 0;
    
    return {arr, sorted};
}
```

## Explanation
The code starts by taking the size of the array. Then a double loop is used to compare the adjacent elements and swap them if they are in the wrong order. Finally, the Iverson condition is used to check if the array is sorted and assign a value of 0 (False) or 1 (True).