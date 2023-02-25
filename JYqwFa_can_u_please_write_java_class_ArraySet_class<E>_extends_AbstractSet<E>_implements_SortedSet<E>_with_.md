

# **ArraySet Class<E> Extending AbstractSet<E> Implementing SortedSet<E>**

ArraySet is a collection of unique elements in sorted order. It provides a fast access to its elements based on the index of the element.

## **Complexity Analysis**

|  Operation  |  Time Complexity |
|:-----------:|:----------------:|
|    `add`    |      `O(n)`     |
|   `remove`  |      `O(n)`     |
|  `contains` |      `O(n)`     |
|  `size`     |      `O(1)`     |
| `iterator`  |      `O(1)`     |

## **Java Implementation**

```java
public class ArraySet<E> extends AbstractSet<E> implements SortedSet<E> {

    // array to store all the elements in the set
    private E[] elements;

    // the size of the set
    private int size;

    // the comparator used to sort the elements in the set
    Comparator<? super E> comparator = null;

    /**
     * Constructs a new ArraySet with the given comparator.
     *
     * @param comparator The comparator used to sort the elements in the set.
     */
    public ArraySet(Comparator<? super E> comparator) {
        this.comparator = comparator;
        elements = (E[]) new Object[10];
        size = 0;
    }

    /**
     * Adds the given element to the set if it is not already present.
     * 
     * @param element The element to be added to the set.
     * @return true if the element was added, false otherwise.
     */
    public boolean add(E element) {
        if (contains(element)) {
            return false;
        }
        if (size == elements.length) {
            resize();
        }
        elements[size++] = element;
        Arrays.sort(elements, 0, size, comparator);
        return true;
    }

    /**
     * Removes the given element from the set if it is present.
     * 
     * @param element The element to be removed from the set.
     * @return true if the element was removed, false otherwise.
     */
    public boolean remove(Object element) {
        for (int i = 0; i < size; i++) {
            if (elements[i].equals(element)) {
                elements[i] = elements[size - 1];
                elements[size - 1] = null;
                size--;
                return true;
            }
        }
        return false;
    }

    /**
     * Returns true if the given element is present in the set.
     * 
     * @param element The element that is to be checked.
     * @return true if the element is present, false otherwise.
     */
    public boolean contains(Object element) {
        for (int i = 0; i < size; i++) {
            if (elements[i].equals(element)) {
                return true;
            }
        }
        return false;
    }

    /**
     * Returns the size of the set.
     * 
     * @return the size of the set.
     */
    public int size() {
        return size;
    }

    /**
     * Returns an iterator over the elements in the set in sorted order.
     * 
     * @return an iterator over the elements in the set in sorted order.
     */
    public Iterator<E> iterator() {
        return new ArraySetIterator();
    }

    /**
     * Inner class implementing the iterator over the elements in the set.
     */
    private class ArraySetIterator implements Iterator<E> {

        // the index of the current element
        private int index = 0;

        /**
         * Returns true if there is a next element to iterate over.
         * 
         * @return true if there is a next element to iterate over.
         */
        public boolean hasNext() {
            return index < size;
        }

        /**
         * Returns the next element in the set.
         * 
         * @return the next element in the set.
         */
        public E next() {
            return elements[index++];
        }
    }

    /**
     * Doubles the size of the array to accommodate more elements.
     */
    private void resize() {
        elements = Arrays.copyOf(elements, elements.length * 2);
    }

}
```