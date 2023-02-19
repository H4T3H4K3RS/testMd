

# **Bubble Sort Algorithm with `vector<int>` as parameter**

The Bubble Sort Algorithm is a sorting algorithm that iteratively compares adjacent elements of a collection, swaps them if they are out of order, and continues until the collection is sorted. Given a collection of numbers stored in a vector, this algorithm can be used to sort the numbers in ascending order.

## **Algorithm**

The pseudocode for the Bubble Sort Algorithm is as follows:

```
procedure bubbleSort(A : list of sortable items):
    n = length(A)
    repeat
        swapped = false
        for i = 1 to n-1 inclusive do
            if A[i-1] > A[i] then
                swap(A[i-1], A[i])
                swapped = true
            end if
        end for
    until not swapped
end procedure
```

## **Implementation**

The following is a C++ implementation of the Bubble Sort Algorithm using a `vector<int>` as a parameter:

```c++
void bubbleSort(vector<int>& A) {
    int n = A.size();
    bool swapped;
    do {
        swapped = false;
        for (int i = 1; i <= n-1; i++) {
            if (A[i-1] > A[i]) {
                swap(A[i-1], A[i]);
                swapped = true;
            }
        }
    } while (swapped);
}
```