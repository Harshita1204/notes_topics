# Time Complexity: Upper Bound, Lower Bound and Tight Bound

1) Upper Bound

Definition:
Upper bound tells us the maximum time an algorithm can take.

It guarantees:
The algorithm will not take more than this time.

Notation:
Big-O notation  
O()

Example: Linear Search

Worst case:
- Element not present
- All elements are checked

Time Complexity:
O(n)

So O(n) is the upper bound.

--------------------------------------------------

2) Lower Bound

Definition:
Lower bound tells us the minimum time an algorithm must take.

It guarantees:
The algorithm cannot run faster than this.

Notation:
Big-Omega notation  
Ω()

Example: Linear Search

Best case:
- Element found at first index

Time Complexity:
Ω(1)

So Ω(1) is the lower bound.

--------------------------------------------------

3) Tight Bound

Definition:
When upper bound and lower bound are the same, we use Theta notation.

Notation:
Θ()

It represents the exact growth rate of the algorithm.

--------------------------------------------------

Example: Traversing an Array

for(int i = 0; i < n; i++) {
    cout << arr[i];
}

This loop always runs n times.

Upper Bound  = O(n)  
Lower Bound  = Ω(n)  
Tight Bound  = Θ(n)

--------------------------------------------------

 Examples:

Linear Search
Best Case  = Ω(1)
Worst Case = O(n)

Binary Search
Best Case  = Ω(1)
Worst Case = O(log n)

Array Deletion
Best Case  = Ω(1)
Worst Case = O(n)

--------------------------------------------------

