

# **Shell (Tsiura) Sort**
Shell Sort is a simple sorting algorithm based on the **Insertion Sort** algorithm. It improves upon insertion sort by breaking the original list into a number of smaller sublists, each of which is sorted using an **Insertion Sort**.

## **Algorithm**
1. Choose a `gap` value to divide the list into sublists.
2. Sort each sublist using insertion sort.
3. Decrease the `gap` value and repeat steps 1 and 2 until the `gap` is 1.
4. Sort the entire list using insertion sort.

## **Pseudocode**
```
procedure shellSort(list : array of items)
   gap := length(list) // Initialize gap
   while gap > 1
      gap := floor(gap / 2)
      for i = gap .. length(list) - 1
         temp := list[i]
         j := i
         while j >= gap and list[j - gap] > temp
            list[j] := list[j - gap]
            j := j - gap
         list[j] := temp
      end while
   end while
end procedure
```

## **C++ Implementation**
```C++
// C++ program for Shell Sort 
#include <iostream> 
#include <vector> 

using namespace std; 

/* function to sort arr using shellSort */
void shellSort(vector<int> &arr) 
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
			
			// put temp (the original a[i]) in its correct location 
			arr[j] = temp; 
		} 
	} 
} 

// Driver code 
int main() 
{ 
	vector<int> arr = {7, 3, 5, 8, 9, 1, 2}; 

	cout << "Array before sorting: "; 
	for (int i = 0; i < arr.size(); i++) 
		cout << arr[i] << " "; 
	cout << endl; 

	shellSort(arr); 

	cout << "Array after sorting: "; 
	for (int i = 0; i < arr.size(); i++) 
		cout << arr[i] << " "; 
	cout << endl; 

	return 0; 
} 
```

## **Time Complexity**
The time complexity of Shell Sort can be expressed as:

$O(n^2)$