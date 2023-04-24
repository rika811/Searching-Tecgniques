# Searching-Techniques

Searching is the process of finding a particular item in a collection of items. A search typically answers whether the item is present in the collection or not. Searching requires a key field such as name, ID, code which is related to the target item. When the key field of a target item is found, a pointer to the target item is returned. The pointer may be an address, an index into a vector or array, or some other indication of where to find the target. If a matching key field isn’t found, the user is informed.

The most common searching algorithms are:

+ Binary search
+ Sequential search

## Sequential search

In this search algorithm a sequential search is made over all the items one by one to search for the targeted item. Each item is checked in sequence until the match is found. If the match is found, particular item is returned otherwise the search continues till the end.

### Algorithm

```
LinearSearch ( Array A, Value x)

Step 1: Set i to 1

Step 2: if i > n then go to step 7

Step 3: if A[i] = x then go to step 6

Step 4: Set i to i + 1

Step 5: Go to Step 2

Step 6: Print Element x Found at index i and go to step 8

Step 7: Print element not found

Step 8: Exit
```

### Binary Search 
Binary Search Algorithm is fast according to run time complexity. This algorithm works on the basis of divide and conquer rule. In this algorithm we have to sort the data collection in ascending order first then search for the targeted item by comparing the middle most item of the collection. If match found, the index of item is returned. If the middle item is greater than the targeted item, the item is searched in the sub-array to the left of the middle item. Otherwise, the item is searched for in the sub-array to the right of the middle item. This process continues on the sub-array as well until the size of the sub array reduces to zero.

### Algorithm

```
Step 1: Data list must be ordered list in ascending order.

Step 2: Probe middle of list

Step 3: If target equals list[mid], FOUND.

Step 4: If target < list[mid], discard 1/2 of list between list[mid] and list[last].

Step 5: If target > list[mid], discard 1/2 of list between list[first] and list[mid].

Step 6: Continue searching the shortened list until either the target is found, or there are no elements to probe.

```

OUTPUTS-

**Sequential searching**-

![Screenshot 2023-04-25 at 1 09 36 AM](https://user-images.githubusercontent.com/91966167/234098956-ba75d66a-079f-48f6-854f-a15659f72700.png)

**Binary searching**-

![Screenshot 2023-04-25 at 1 19 39 AM](https://user-images.githubusercontent.com/91966167/234100899-622079a5-469d-40e4-a22f-e618cac13226.png)



