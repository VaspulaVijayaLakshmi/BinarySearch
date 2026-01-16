# BinarySearch


Binary Search is not just about finding an element in a sorted array. It’s a technique that applies to arrays, rotated arrays, and even optimization problems. 


Binary search has two important aspects.

-> A sorted array

-> Splitting an array into two halves. 

If We do not have the first one here try to think if second point can be used on ny parameter.
Eg:PEAK ELEMENT


-> Binary Search Pattern for Problems -  which need  maximize the minimum or mimimise the maximum
________________________




🔹 𝗦𝘁𝗲𝗽 𝟭:  Core

Works only on monotonic conditions (sorted or yes/no search space).

Narrow the range until the answer is found.
Common pitfalls: overflow (mid = low + (high - low)/2), wrong boundaries, infinite loops.


1️ Binary Search – https://lnkd.in/gS6HJ9sJ  
2️ First Bad Version – https://lnkd.in/gYv94xhN  
3️ Guess Number Higher or Lower – https://lnkd.in/gQxMFRuP  
4️ Search Insert Position – https://lnkd.in/ghTEhu68  
5️ Sqrt(x) – https://lnkd.in/grR6Qprg  



______________________________


🔹 𝗦𝘁𝗲𝗽 𝟮: 𝗜𝗻𝘁𝗲𝗿𝗺𝗲𝗱𝗶𝗮𝘁𝗲 – 𝗕𝗶𝗻𝗮𝗿𝘆 𝗦𝗲𝗮𝗿𝗰𝗵 𝗩𝗮𝗿𝗶𝗮𝗻𝘁𝘀

Boundaries – find leftmost/rightmost element.
Rotated Arrays – binary search on two halves.
Peak Finding – search in non-standard monotonic structures.


1️ Find First and Last Position – https://lnkd.in/g3NuHzvM  
2️ Search in Rotated Sorted Array – https://lnkd.in/gt8nYfs4  
3️ Find Peak Element – https://lnkd.in/gXvQvugc  
4️ Find Minimum in Rotated Sorted Array – https://lnkd.in/gTBiuc6x  
5️ Koko Eating Bananas – https://lnkd.in/gCsaZ3hp  

__________________________________



🔹 𝗦𝘁𝗲𝗽 𝟯: 𝗔𝗱𝘃𝗮𝗻𝗰𝗲𝗱 

Here, you’re not finding an index, but the optimal answer in a numeric or conceptual range (min/max resources, distance, capacity).


1️ Capacity to Ship Packages – https://lnkd.in/gNcxa9nx  
2️ Divide Chocolates – 1231. Divide Chocolate  
3️ Find Smallest Divisor given threshold – 1283. Find the Smallest Divisor Given a Threshold  
4️ Minimum Absolute Sum Difference – 1818. Minimum Absolute Sum Difference  
5️ Minimum Number of Days to Make m Bouquets – 1482. Minimum Number of Days to Make m Bouquets  
6️ Longest Subsequence With Limited Sum – 2389. Longest Subsequence With Limited Sum


Hard:

1️ Median of Two Sorted Arrays – https://lnkd.in/g7dV4DcJ  
2️ Split Array Largest Sum – https://lnkd.in/gxjnTK7m  
3️ Aggressive Cows (GFG/LC variant) – https://lnkd.in/gqGF9KmH  
4️ K-th Smallest Pair Distance – https://lnkd.in/g4yAeSq8  
5️ Painters Partition  
6️ Allocate Pages of Boo

Solve Painters Partition before Allocate Pages of Book




_____________________


-> Observation :

 Search in Rotated Sorted Array – https://lnkd.in/gt8nYfs4  
 Find Minimum in Rotated Sorted Array – https://lnkd.in/gTBiuc6x  

Difference between the two problems:

-> Find Minimum → we don’t care about the exact value, only about the minimum. So we can keep shrinking until l == r.

-> Search Target → we need to decide: is the target in the left half or the right half?
That requires extra comparisons with the target, not just nums[mid] vs nums[end].



-> Binaru Search can be applied when we do sorting and then in the search spae we need to check something.
LIke max/min.


-> 1482. Minimum Number of Days to Make m Bouquets -  Attention to detail - consecutive flowers to make boque, lets say we need to collect 5 cons. flowers
if we collect flowers 4 flowers cons and 5th day bloom=0, then we need to throw these flowers. and strt colectig again




Key difference from Chocolate Division

Chocolate: canDivide checks if each piece ≥ mid (maximize min).
Books: canAllocate checks if each piece ≤ mid (minimize max).



_____________________________________

******IMP
Minimize Max Distance to Gas Station



In integer binary search, we stop when l <= r crosses.
But in doubles/fractions, the search space never “crosses” perfectly — it keeps shrinking but never hits the exact answer.

So we stop when the search space (h - l) becomes very small (like 1e-6).
That’s our precision tolerance.

_______________________________________



1. Contiguous → Greedy
2. Unrestricted → Backtracking

-> 2305. Fair Distribution of Cookies - Backtracking Approach

This doesnt work with BS, as there is no conitguos restraint
_________________



One-line intuition

Ship packages → minimize max → <= cap
->->->
Divide chocolate → maximize min → >= mid


-> Divide Cholate:

Can we make at least K+1 pieces each having sweetness ≥ mid ?

We want to check:
Can we make at least K+1 pieces each having sweetness ≥ mid ?


-> Ship Package
Can we mke the capacity kess and less...
So we check the condiition capcit< mid

______

```
Minimize max → “avoid overflow” → split when >

Maximize min → “ensure minimum” → cut when >=
```


