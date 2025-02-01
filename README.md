# 🔥 10 Must-Know Patterns to Master LeetCode 🔥  

Each pattern includes actual LeetCode problems so you can practice immediately!  

---

## ✅ 1) Sliding Window – The Secret to Optimizing Subarrays  
### When to use it?  
- If the problem involves **subarrays, substrings, or continuous data**, think **Sliding Window**!  
- Instead of using **O(n²) brute force**, this method allows you to "slide" over the data efficiently.  

### Example Problems:  
- [Longest Substring Without Repeating Characters](https://leetcode.com/problems/longest-substring-without-repeating-characters/)  
- [Minimum Size Subarray Sum](https://leetcode.com/problems/minimum-size-subarray-sum/)  
- [Permutation in String](https://leetcode.com/problems/permutation-in-string/)  
- [Longest Repeating Character Replacement](https://leetcode.com/problems/longest-repeating-character-replacement/)  

### How I learned it:  
I first used brute force to check all substrings, but then I learned to **expand and shrink the window dynamically** to optimize!  

---

## ✅ 2) Two Pointers – The Ultimate Trick for Sorted Arrays  
### When to use it?  
- If a problem involves **pairs, sorted arrays, or linked lists**, think **Two Pointers**!  
- Instead of nested loops (**O(n²)**), move two pointers to reduce complexity to **O(n)**.  

### Example Problems:  
- [Two Sum II - Input Array is Sorted](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/)  
- [Valid Palindrome](https://leetcode.com/problems/valid-palindrome/)  
- [3Sum](https://leetcode.com/problems/3sum/)  
- [Container With Most Water](https://leetcode.com/problems/container-with-most-water/)  

### How I learned it:  
I kept using a hashmap for everything—until I realized some problems don’t need extra space. **Moving two pointers inward was a game-changer!**  

---

## ✅ 3) Fast & Slow Pointers – Cycle Detection in Disguise  
### When to use it?  
- If a problem asks about **finding a cycle or middle node in a linked list**, think **Fast & Slow Pointers**!  
- The slow pointer moves **one step**, fast pointer moves **two steps**—if they meet, there’s a cycle.  

### Example Problems:  
- [Linked List Cycle](https://leetcode.com/problems/linked-list-cycle/)  
- [Find the Duplicate Number](https://leetcode.com/problems/find-the-duplicate-number/)  
- [Middle of the Linked List](https://leetcode.com/problems/middle-of-the-linked-list/)  
- [Happy Number](https://leetcode.com/problems/happy-number/)  

### How I learned it:  
I initially used **hash sets** for cycle detection, but it used **extra space**. **Floyd’s Tortoise and Hare Algorithm** made my solutions much more efficient!  

---

## ✅ 4) Merge Intervals – Mastering Overlapping Ranges  
### When to use it?  
- If a problem involves **overlapping intervals** (e.g., **calendars, schedules, time ranges**), **sort and merge them!**  

### Example Problems:  
- [Merge Intervals](https://leetcode.com/problems/merge-intervals/)  
- [Insert Interval](https://leetcode.com/problems/insert-interval/)  
- [Meeting Rooms II](https://leetcode.com/problems/meeting-rooms-ii/)  
- [Non-overlapping Intervals](https://leetcode.com/problems/non-overlapping-intervals/)  

### How I learned it:  
I used to manually check each interval one by one—**big mistake!** Sorting first makes merging much easier.  

---

## ✅ 5) Binary Search – More Than Just Sorted Arrays  
### When to use it?  
- If a problem involves **sorted data** or requires you to **search for a value**, **Binary Search** is your friend.  
- Also useful for **"Binary Search on Answer"** problems (e.g., **minimizing/maximizing values**).  

### Example Problems:  
- [Binary Search](https://leetcode.com/problems/binary-search/)  
- [Search in Rotated Sorted Array](https://leetcode.com/problems/search-in-rotated-sorted-array/)  
- [Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/)  
- [Find Peak Element](https://leetcode.com/problems/find-peak-element/)  

### How I learned it:  
I thought Binary Search was just for searching numbers—but it’s also great for **finding optimal solutions in range-based problems!**  

---

## ✅ 6) BFS – The Go-To for Shortest Paths  
### When to use it?  
- If a problem requires **level-order traversal** or **shortest paths**, BFS is usually the best choice.  

### Example Problems:  
- [Word Ladder](https://leetcode.com/problems/word-ladder/)  
- [Binary Tree Level Order Traversal](https://leetcode.com/problems/binary-tree-level-order-traversal/)  
- [Shortest Path in Binary Matrix](https://leetcode.com/problems/shortest-path-in-binary-matrix/)  
- [Rotting Oranges](https://leetcode.com/problems/rotting-oranges/)  

### Pro Tip:  
Use a **queue** for BFS to explore nodes **level by level**.  

---

## ✅ 7) DFS – When You Need to Explore Everything  
### When to use it?  
- If a problem requires **recursion, backtracking, or deep exploration**, **DFS** is your answer!  

### Example Problems:  
- [Number of Islands](https://leetcode.com/problems/number-of-islands/)  
- [Word Search](https://leetcode.com/problems/word-search/)  
- [Clone Graph](https://leetcode.com/problems/clone-graph/)  
- [Surrounded Regions](https://leetcode.com/problems/surrounded-regions/)  

### How I learned it:  
DFS was intimidating at first, but once I saw it as **recursive tree traversal**, it clicked!  

---

## ✅ 8) Dynamic Programming – Avoiding Repeated Work  
### When to use it?  
- If a problem has **overlapping subproblems**, use **memoization or tabulation**.  

### Example Problems:  
- [House Robber](https://leetcode.com/problems/house-robber/)  
- [Climbing Stairs](https://leetcode.com/problems/climbing-stairs/)  
- [Longest Common Subsequence](https://leetcode.com/problems/longest-common-subsequence/)  
- [Coin Change](https://leetcode.com/problems/coin-change/)  

### How I learned it:  
DP used to scare me—until I started **thinking recursively first**, then optimizing with a cache (**memoization**)!  

---

## ✅ 9) Backtracking – Trying All Possibilities, Efficiently  
### When to use it?  
- If a problem involves **combinations, permutations, or constraints**, use **backtracking!**  

### Example Problems:  
- [N-Queens](https://leetcode.com/problems/n-queens/)  
- [Sudoku Solver](https://leetcode.com/problems/sudoku-solver/)  
- [Permutations](https://leetcode.com/problems/permutations/)  
- [Subsets](https://leetcode.com/problems/subsets/)  

### How I learned it:  
I used to write **brute-force loops**, but learning **pruning and constraints** helped me optimize my solutions!  

---

## ✅ 10) Heaps/Priority Queue – When Sorting Isn’t Fast Enough  
### When to use it?  
- If a problem asks for the **top K elements** or **dynamic sorting**, think **Heaps/Priority Queue!**  

### Example Problems:  
- [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array/)  
- [Merge K Sorted Lists](https://leetcode.com/problems/merge-k-sorted-lists/)  
- [Find Median from Data Stream](https://leetcode.com/problems/find-median-from-data-stream/)  
- [Task Scheduler](https://leetcode.com/problems/task-scheduler/)  
