# LJ Code 401 - Week 7
[`Home`](../README.md) [`401 Index`](401_README.md)
<hr>

#### [Sorting](https://en.wikipedia.org/wiki/Sorting_algorithm) 

###### insertion sort
inserts each value into the new collection where it would be, navigating up or down

###### selection sort -> heap sort
uses a heap to select the smallest value and insert it into a new collection

###### bubble sort
inserts each value into the collection one at a time, if no values are moved, the sort stops

###### quick sort
divide and conquer, sort collection my division
```
5        11       13*        19        4       9
5 < 13* | 11 < 13* | 19 > 13* | 4 < 13* | 9 < 13*
9,    4,    11*,    5,    13,   19
            5, 4, 9, < 11* <      13, 19
            4* < 5 < 9
  [4, 5, 9, 11, 13, 19]
```
\* = pivot

###### merge sort
breaks down components and sorts the values one at a time
```
5        11       13    |    19        4       9
    5, 11, 13                     19, 4, 9
  5,      11, 13              19,       4, 9
        11      13                    4      9

  [11, 13]          |           [4, 9]        
  [5, 11, 13]       |           [4, 9, 19]        
  [4, 5, 9, 11, 13, 19]        
```

###### in-place
sorts the collection without creating a copy

###### stable
sorts the collection while keeping duplicates in the same order as they were
