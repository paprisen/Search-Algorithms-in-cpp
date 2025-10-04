# Search-Algorithms-in-cpp

Aim: To study different searching techniques in C++ and implement programs to search for elements in an array.

Tools: VS Code

## Theory

Searching Algorithms are fundamental algorithms used to locate specific elements within data structures. They are essential building blocks in computer science for data retrieval, database operations, and information processing. Understanding different searching techniques helps in choosing the most efficient approach based on data organization and performance requirements.

## Key Concepts:

* Search Operation: The process of finding a particular element in a collection of data.
```
int search(int arr[], int size, int target) {
    // Search logic implementation
    return index; // or -1 if not found
}
```

* Search Key: The element or value being searched for in the data structure.

```
int target = 10;  // This is our search key
```

* Search Space: The collection of elements where the search operation is performed.

```
int arr[] = {5, 3, 8, 4, 2};  // This is our search space
```

* Time Complexity: The measure of efficiency in terms of operations required relative to input size.

## Searching Algorithm Categories:

```
// Basic search pattern
int search_algorithm(data_structure, search_key) {
    // Implementation specific to algorithm
    if (element_found) {
        return position;
    }
    return -1; // Not found
}
```

## Types of Searching:

* Linear/Sequential Search: Examines elements one by one from start to end

* Binary Search: Divides search space in half repeatedly (requires sorted data)

* Hash-based Search: Uses hash functions for direct access

* Tree-based Search: Utilizes tree structures for hierarchical searching

* Interpolation Search: Estimates position based on key value distribution

* Jump Search: Skips elements in fixed intervals then performs linear search

## Program 1: Linear Search

## Logic:

A function is created to search for the element in the array. The function iterates over all elements sequentially. Returns the index if the element is found, otherwise returns -1.

## Algorithm:

1. Start

2. Input the size of the array.

3. Input the array elements.

4. Input the element to be searched.

5. Iterate through the array:

6. If element matches, return its index.

7. Else continue.

8. If not found, return -1.

9. End

## Program 2: Sequential Search[Linear in main]

## Logic:

The search is performed directly inside the main() function using a loop. A boolean flag keeps track of whether the element is found. If found, the index is printed; otherwise, a “not found” message is displayed.

## Algorithm:

1. Start

2. Input the number of elements.

3. Input the array elements.

4. Input the element to be searched.

5. Initialize a flag as false.

6. Iterate through the array:

7. If element matches, print index and set flag true.

8. Break loop.

9. If flag remains false, print element not found.

10. End

## Program 3: Binary Search

## Logic:

The array must be sorted. Two pointers (left and right) are used to track the current search interval. The middle element is compared with the target element. Depending on comparison, the search continues in the left or right half.

## Algorithm:

1. Start

2. Input the number of elements.

3. Input the sorted array elements.

4. Input the element to be searched.

5. Initialize left = 0 and right = size-1.

6. While left <= right:

7. Calculate mid = (left + right)/2.

8. If arr[mid] matches, return index.

9. If arr[mid] < element, search in right half (left = mid+1).

10. Else search in left half (right = mid-1).

11. If element not found, return -1.

12. End

## Conclusion

Linear and binary search are fundamental searching techniques. Linear search is simple and works on any array, while binary search is more efficient for sorted arrays. Understanding these methods is essential for designing efficient algorithms for data retrieval.
