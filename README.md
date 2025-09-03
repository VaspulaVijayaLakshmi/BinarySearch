# BinarySearch


Binary Search is not just about finding an element in a sorted array. It’s a technique that applies to arrays, rotated arrays, and even optimization problems. 


Binary search has two important aspects.

-> A sorted array

-> Splitting an array into two halves. 

If We do not have the first one here try to think if second point can be used on ny parameter.
Eg:PEAK ELEMENT




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

1️ Median of Two Sorted Arrays – https://lnkd.in/g7dV4DcJ  
2️ Split Array Largest Sum – https://lnkd.in/gxjnTK7m  
3️ Aggressive Cows (GFG/LC variant) – https://lnkd.in/gqGF9KmH  
4️ Capacity to Ship Packages – https://lnkd.in/gNcxa9nx  
5️ K-th Smallest Pair Distance – https://lnkd.in/g4yAeSq8 






_____________________


-> Observation :

 Search in Rotated Sorted Array – https://lnkd.in/gt8nYfs4  
 Find Minimum in Rotated Sorted Array – https://lnkd.in/gTBiuc6x  

Difference between the two problems:

Find Minimum → we don’t care about the exact value, only about the minimum. So we can keep shrinking until l == r.

Search Target → we need to decide: is the target in the left half or the right half?
That requires extra comparisons with the target, not just nums[mid] vs nums[end].



Binaru Search can be applied when we do sorting and then in the search spae we need to check something.
LIke max/min.
