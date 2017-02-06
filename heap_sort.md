# Heap Sort

need to create a max heap from unsorted array
and then heapify
----
good for queues
big O(n*logn) runtime 
	-best and worst case is same
-better than quick sort because worst case quick sort is O(n^2)

---
all parents greater than children (max heap)

array from top to bottom and left to right

after create max heap - switch first and last value (creating a sorted array inside of same location)

---
build max heap() is O(n)
max-heapify function is O(logn) 
	-every time bring value down tree you are dividing decisions by two (hence logn)

-not a stable sort (does not retrieve same order each time)

1. call max heap function and builds tree with largest element at top
2. swap top with bottom creating a sorted array of size 1 and reducing size of heap by 1
3. recursively or iteratively call max heapify function on first element and get largest element at top
4. swap top with bottom again and fix the heap
5. continue until heap is 1 item and we have sorted list(can sort descending or ascending)

MaxHeapify() extra-pseudocode
	compare current value at top with children and if children are larger swap with larger of children

example:
1,2,3,4,5,6,7,8,9
