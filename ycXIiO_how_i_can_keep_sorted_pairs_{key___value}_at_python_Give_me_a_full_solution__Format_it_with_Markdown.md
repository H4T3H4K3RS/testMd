

Solution

**Sorted Pairs {Key - Value} in Python**

Sorted pairs can be kept in Python using a `dictionary`. A dictionary is a data structure that stores data in key-value pairs. The keys of a dictionary must be unique and of an immutable data type such as a `string`, `integer`, or `tuple`. The values of a dictionary can be of any data type.

A dictionary can be initialized in Python using the `dict()` function. For example, the following code creates an empty dictionary:

```python
d = dict()
```

To add key-value pairs to a dictionary, the `[key]` syntax can be used. For example, the following code adds a key-value pair to the dictionary:

```python
d[key] = value
```

To keep the dictionary sorted, the `sorted()` function can be used. The `sorted()` function takes in a dictionary and returns a list of tuples, where each tuple contains a key-value pair from the dictionary. For example, the following code sorts the dictionary by keys:

```python
sorted_d = sorted(d.items(), key=lambda x: x[0])
```

The list of tuples can then be printed to see the sorted key-value pairs. For example, the following code prints the sorted key-value pairs:

```python
for key, value in sorted_d:
    print(key, value)
```

**Conclusion**

In Python, sorted pairs can be kept using a dictionary and the `sorted()` function. The `dict()` function can be used to initialize an empty dictionary, and the `[key]` syntax can be used to add key-value pairs to the dictionary. The `sorted()` function can then be used to sort the dictionary, and the sorted key-value pairs can be printed.