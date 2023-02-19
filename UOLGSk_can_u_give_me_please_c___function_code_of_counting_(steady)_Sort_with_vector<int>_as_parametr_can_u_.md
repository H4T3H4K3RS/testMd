

**Solution**

The following is a C++ function code for counting sort with `vector<int>` as the parameter. The code is commented to explain each line.

```C++
// countSort() is a function that sorts a vector of integers using the Counting Sort algorithm
void countSort(vector<int>& v) 
{ 
    // Find the maximum and minimum elements in the vector.
    int max = *max_element(v.begin(), v.end()); 
    int min = *min_element(v.begin(), v.end()); 
  
    // Create a vector to store the count of each element  
    // Range is from min to max  
    int range = max - min + 1; 
    vector<int> count(range); 
  
    // Store the count of each elements in count[]  
    for (int i = 0; i < v.size(); i++) 
        count[v[i] - min]++; 
  
    // Change count[i] so that count[i] now contains actual  
    // position of this element in the output vector 
    for (int i = 1; i < count.size(); i++) 
        count[i] += count[i - 1]; 
  
    // Build the output vector 
    vector<int> output(v.size()); 
    for (int i = v.size() - 1; i >= 0; i--) 
    { 
        output[count[v[i] - min] - 1] = v[i]; 
        count[v[i] - min]--; 
    } 
  
    // Copy the output vector to v[] so that v[] now 
    // contains sorted elements
    for (int i = 0; i < v.size(); i++) 
        v[i] = output[i]; 
} 
```