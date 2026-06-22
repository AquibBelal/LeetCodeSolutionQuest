# LeetCode Pattern Recognition System

One of the biggest improvements you can make in DSA is to stop thinking:

> "What is the solution?"

and start thinking:

> "What pattern is this problem?"

Most LeetCode problems are variations of about **15-20 major patterns**.

---

# Step 1: Read the Constraints First

The constraints often tell you the expected complexity.

| n | Expected Complexity |
|---|---|
| `n ≤ 10` | `O(n!)` or `O(2ⁿ)` |
| `n ≤ 20` | Backtracking / Bitmask |
| `n ≤ 100` | `O(n²)` |
| `n ≤ 1000` | `O(n²)` or `O(n log n)` |
| `n ≤ 10⁵` | `O(n log n)` or `O(n)` |
| `n ≤ 10⁶` | `O(n)` |

### Example

```text
n = 100000
```

Immediately eliminate:

❌ `O(n²)`

Think:

✅ Hashing  
✅ Sliding Window  
✅ Monotonic Stack  
✅ Greedy  
✅ Binary Search

---

# Step 2: Look for Keywords

---

# 1. Hashing (Set / Dictionary)

## Keywords

```text
duplicate
frequency
count occurrences
pair sum
unique elements
anagrams
missing numbers
```

## Questions

- Two Sum
- Set Mismatch
- Contains Duplicate
- Valid Anagram
- Find All Numbers Disappeared

## Mental Trigger

```text
Need fast lookup?
Need to remember seen elements?

→ Hashing
```

---

# 2. Two Pointers

## Keywords

```text
sorted array
pair
triplet
palindrome
container
remove duplicates
```

## Questions

- Two Sum II
- 3Sum
- Container With Most Water
- Valid Palindrome

## Mental Trigger

```text
Array is sorted?
Need left and right indices?

→ Two Pointers
```

---

# 3. Sliding Window

## Keywords

```text
subarray
substring
longest
smallest
at most k
exactly k
consecutive
window
```

## Questions

- Longest Substring Without Repeating Characters
- Maximum Average Subarray
- Minimum Size Subarray Sum

## Mental Trigger

```text
Contiguous portion of array/string?

→ Sliding Window
```

---

# 4. Prefix Sum

## Keywords

```text
range sum
sum between indices
subarray sum
running total
```

## Questions

- Range Sum Query
- Subarray Sum Equals K
- Pivot Index

## Mental Trigger

```text
Need many sum calculations?

→ Prefix Sum
```

---

# 5. Monotonic Stack

## Keywords

```text
next greater
next smaller
previous greater
previous smaller
first element to left/right
discount
temperature
span
histogram
```

## Questions

- Daily Temperatures
- Final Prices With a Special Discount in a Shop
- Next Greater Element
- Online Stock Span
- Largest Rectangle in Histogram

## Mental Trigger

```text
First greater/smaller element?

→ Monotonic Stack
```

---

# 6. Binary Search

## Keywords

```text
sorted
minimum possible
maximum possible
search space
answer lies between
kth smallest
```

## Questions

- Search Insert Position
- Koko Eating Bananas
- Capacity To Ship Packages Within D Days

## Mental Trigger

```text
Can answer be guessed and verified?

→ Binary Search on Answer
```

---

# 7. Greedy

## Keywords

```text
minimum operations
maximum profit
intervals
jump
gas station
```

## Questions

- Jump Game
- Gas Station
- Non-overlapping Intervals

## Mental Trigger

```text
Can local best lead to global best?

→ Greedy
```

---

# 8. Backtracking

## Keywords

```text
all combinations
all permutations
generate
every possibility
subsets
N-Queens
```

## Questions

- Permutations
- Subsets
- Combination Sum
- Letter Combinations of a Phone Number

## Mental Trigger

```text
Need ALL possible answers?

→ Backtracking
```

---

# 9. Dynamic Programming

## Keywords

```text
maximum/minimum
count ways
longest
can we reach
optimal answer
```

## Questions

- House Robber
- Coin Change
- Climbing Stairs
- Longest Increasing Subsequence

## Mental Trigger

```text
Problem depends on smaller subproblems?

→ Dynamic Programming
```

---

# 10. Breadth-First Search (BFS)

## Keywords

```text
shortest path
minimum steps
levels
nearest
infection
distance
```

## Questions

- Rotting Oranges
- Word Ladder
- Binary Tree Level Order Traversal

## Mental Trigger

```text
Need minimum steps?

→ BFS
```

---

# 11. Depth-First Search (DFS)

## Keywords

```text
explore
connected components
islands
paths
tree traversal
```

## Questions

- Number of Islands
- Clone Graph
- Path Sum

## Mental Trigger

```text
Need to explore everything?

→ DFS
```

---

# 12. Union Find (Disjoint Set Union)

## Keywords

```text
connected
friend circles
groups
components
network
```

## Questions

- Number of Provinces
- Accounts Merge
- Redundant Connection

## Mental Trigger

```text
Need to merge groups?

→ DSU
```

---

# 13. Heap / Priority Queue

## Keywords

```text
top k
kth largest
smallest element
median
merge sorted
```

## Questions

- Kth Largest Element in an Array
- Top K Frequent Elements
- Find Median from Data Stream

## Mental Trigger

```text
Need repeated min/max?

→ Heap
```

---

# 14. Interval Problems

## Keywords

```text
meetings
ranges
overlapping
merge intervals
schedule
```

## Questions

- Merge Intervals
- Meeting Rooms
- Insert Interval

## Mental Trigger

```text
Ranges?

→ Sort + Intervals
```

---

# 15. Graph

## Keywords

```text
courses
dependencies
prerequisites
routes
network
```

## Questions

- Course Schedule
- Network Delay Time
- Reconstruct Itinerary

## Mental Trigger

```text
Things connected by edges?

→ Graph
```

---

# Personal Recognition Flow

```text
Problem
│
├── Need fast lookup?
│      → Hashing
│
├── Sorted?
│      → Two Pointers / Binary Search
│
├── Subarray/Substring?
│      → Sliding Window / Prefix Sum
│
├── First greater/smaller?
│      → Monotonic Stack
│
├── Top K?
│      → Heap
│
├── Intervals?
│      → Sort + Intervals
│
├── Tree?
│      → DFS/BFS
│
├── Connected components?
│      → DFS/BFS/DSU
│
├── Minimum steps?
│      → BFS
│
├── All possibilities?
│      → Backtracking
│
└── Optimal answer from smaller answers?
       → Dynamic Programming
```

---

# Interview Cheat Sheet

| Clue | Pattern |
|------|----------|
| Duplicate/Frequency | Hashing |
| Sorted Array | Two Pointers |
| Subarray/Substring | Sliding Window |
| Range Sum | Prefix Sum |
| First Greater/Smaller | Monotonic Stack |
| Top K | Heap |
| Minimum Steps | BFS |
| Connected Components | DFS/DSU |
| Generate All | Backtracking |
| Count Ways | Dynamic Programming |
| Search Space | Binary Search |
| Intervals | Sort + Intervals |

---

# Recommended Study Order

```text
Arrays
↓
Hashing
↓
Two Pointers
↓
Sliding Window
↓
Stack & Monotonic Stack
↓
Binary Search
↓
Trees
↓
Graphs
↓
Heap
↓
Backtracking
↓
Dynamic Programming
```

This progression builds patterns on top of each other and makes recognizing new problems much easier.
