### **Ammar Ahmad**
* **Round**: Technical Interview
* **Discussion**: Introduction, project discussion, and C++ fundamentals.

1.  **Aptitude Question**: A king has 10 gold bars (10kg each). He assigns 10 people to make 10 1kg bars from each 10kg bar. One person steals 100gm from each 1kg bar they make. The king has a weighing scale he can use only once. How can he find the robber?
    * **Solution**: Take 1 bar from person #1, 2 bars from person #2, 3 from #3, and so on, up to 10 bars from person #10.
    * Weigh all these collected bars together. The expected weight is `(1+2+...+10) * 1kg = 55kg`.
    * The deficit from 55kg will reveal the thief. If the weight is `300gm` less than expected, person #3 is the thief (since they contributed 3 bars, each 100gm lighter).

2.  **DSA Question**: Merge a linked list into another at two specified indices.

---

### **Akhand Singh**
* **Interviewer**: Tushark
* **Round**: Technical Interview
* **Discussion**: Intro & Project (10 mins), Database (30 mins), DSA (15 mins)

#### **Database Questions**
1.  What is **Sharding** and how do you implement it?
2.  What is the time complexity for finding data using **prime indexing**?
3.  How would you implement prime indexing? (`O(1)` vs `O(log n)`).
4.  What are **collisions** in hashing? How can you reduce the time to resolve them?
    * **Hint**: A common method is using a linked list for the same key. How can you optimize the worst-case `O(N)` of this approach? (e.g., using a balanced BST or another hash map).
5.  How would you implement a `set` data structure?
6.  What are the different types of **indexing**? How can they be implemented in C++?

#### **DSA Question**
1.  Generate a sorted array of all subsequences of a given string. The solution should not use recursion stack space.
    * **Solution Approach**: Bitmasking.
    * **Follow-up**: Discuss the Time and Space Complexity for both the recursive and bitmasking approaches.

---

### **Yash Kamdar**
* **Round**: Technical Interview

1.  **Problem**: Given an array of 1s and 0s and a set of ranges `(i, j)`, find the number of 0s in each range.
    * **Input Array**: `[1, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 1]`
    * **Ranges**: `[[0,4], [3,6], [1, 5], [0, 7]]`
    * **Output**: `[3, 3, 4, 6]`
    * **Solution**: Use a prefix sum/count array. `prefix_zeros[k]` stores the number of zeros from index 0 to `k-1`. The count for a range `[i, j]` is `prefix_zeros[j+1] - prefix_zeros[i]`.
    * **Follow-ups**:
        * Why did you use a `vector` over a C-style array?
        * When should you use a `vector` vs. an array?
        * How does a `vector` allocate memory dynamically?

2.  **Problem**: Design a stack with a `getMin()` function that operates in `O(1)` time complexity and without using extra space.
    * **Topics**: Standard stack operations (`push`, `pop`), their complexities, and pseudocode.

---

### **Shubhanshi Bishnoi**
* **Round**: 1 (Technical)

1.  **Problem**: Check if a given number is a perfect cube.
    * **Solution**: Discussed both binary search and using the `cbrt()` function.
2.  **Problem**: Given two sorted arrays and a value `x`, find the pair of elements (one from each array) whose sum is closest to `x`.
    * **Solution**: Used a two-pointer approach. Discussed time complexities, including cases where array lengths differ.
3.  **Problem**: You are given an array and can perform an operation `k` times. An operation consists of taking an element `x`, removing it, and inserting `ceil(x/2)` back into the array. Find the minimum possible sum of the array after exactly `k` operations.
    * **Solution**: An `O(k*log(n))` optimal solution uses a max heap (priority queue).

---

### **Anand Kumar**
* **Round**: Technical Interview

1.  **Problem**: [Trim a Binary Search Tree](https://leetcode.com/problems/trim-a-binary-search-tree/description/).
2.  **Theory**: Real-life applications of Stack and Queue.
3.  **Database**: Types of `JOIN` in SQL, focusing on the difference between `INNER JOIN` and `OUTER JOIN`.

---

### **Swayam Jain**
* **Round**: Technical Interview

1.  **Problem**: [Find the largest subarray with 0 sum](https://www.geeksforgeeks.org/find-the-largest-subarray-with-0-sum/).
2.  **OS**: Difference between a **Thread** and a **Process**.
3.  **Data Structures**: Real-life uses of Stack and Queue.
4.  **OOPs**: Function Overloading vs. Function Overriding.
5.  **OOPs**: Different types of access modifiers and their real-life use cases.

---

### **Akash Sinha**
* **Interviewer**: Sonalika
* **Round**: Technical Interview
* **Discussion**: Intro and Project (10 mins)

1.  **Problem**: Implement a `Stack` class with all its standard operations.
    * **Follow-up**: Implement additional operations like `isEmpty()` and `reverse()` the stack with `O(1)` space complexity.
2.  **OOPs**: Discussion on pointers, virtual functions, pure virtual functions, and abstract classes.

---

### **Medha Aggarwal**
* **Round**: Technical Interview
* **Discussion**: Intro and project discussion.

1.  **Problem**: A delivery boy starts at the top-left `(0,0)` of a grid (2D vector) and must reach the bottom-right corner. He can only move right or down. Each cell `(i, j)` has a cost associated with visiting it. Find the minimum cost path to reach the destination.
    * **Solution**: This is a classic Dynamic Programming problem.
    * **Follow-up**: Discuss time complexity and potential optimizations.

---

### **Kashika Aggarwal**
* **Interviewer**: Ashutosh
* **Round**: Technical Interview

1.  **Discussion**: Introduction and a detailed discussion on a specific project from the resume.
2.  **Database**: Differences between **MySQL** and **MongoDB**, their use cases, and ACID properties.
3.  **System Design/DSA**: Design an API that returns the mutual friends between any two users on a social networking site.
    * **Follow-up**: The question evolved into a DSA problem focusing on continuous space and time complexity optimizations for different implementation approaches.
4.  **Data Structures**: Time complexity analysis for insertion in a `stack` and a `hashmap`. How is it calculated?

---

### **Harshit Tomar**
* **Interviewer**: Garima
* **Round**: Technical Interview

1.  **Problem**: Given an array, find the minimum difference between any two elements. Return all pairs that have this minimum difference.
    * **Follow-ups**: Solve it without using a map. Can you reduce the time complexity from `O(n log n)`?
2.  **Problem**: (Same as Shubhanshi's Q3) Given an array and `k` operations, where you can replace any number `x` with `ceil(x/2)`, find the minimum possible array sum.
3.  **OOPs**: What is polymorphism? Provide an example.
4.  **Puzzle**: There are three switches outside a room and three bulbs inside. You can only enter the room once. How do you determine which switch corresponds to which bulb?
    * **Solution**: Flip switch #1 on for a few minutes, then turn it off. Turn switch #2 on. Enter the room. The bulb that is on corresponds to switch #2. The bulb that is off but warm corresponds to switch #1. The remaining cold, off bulb corresponds to switch #3.

---

### **Aakash Shankar Prasad**
* **Round**: Technical Interview 1
* **Discussion**: Intro and project discussion.

1.  **Problem**: Reverse a linked list in groups of size `k`. If the number of remaining nodes at the end is less than `k`, leave them as is.
    * **Follow-ups**:
        * How would you test your program? (e.g., NULL case, single node, `k=1`).
        * How would you handle an extremely large list that exceeds standard data type limits?
        * What is the difference between Function Overriding and Overloading? (asked during coding).
2.  **Database**: What are **SQL Views**? Can you update the original tables through them?
3.  **Database**: Explain **ACID** properties.
4.  **Database**: What is **Indexing**? In which cases is it not beneficial?
5.  **Database**: What is **Partitioning**? How is it different from indexing?
6.  **OS**: If you have 50 computers and need to execute a specific `.exe` file on all of them at exactly 5 PM, how would you automate this?
    * **Hint**: Look into cron jobs (Linux/Mac) or Task Scheduler (Windows).

---

### **Prakhar Shukla**
* **Round**: Technical Interview
* **Discussion**: Project Discussion (10 min)

1.  **Problem**: Find the middle of a linked list.
    * **Follow-up**: When will the tortoise and hare (slow and fast pointer) method not work? (e.g., in a circular linked list without careful cycle detection).
2.  **Database**: Multiple SQL query questions, including subqueries.
3.  **System Design**: In your project, if all users had to be logged out at 5 PM, how would you implement it?

---

### **Divyam Gupta**
* **Interviewer**: Tushar Raina
* **Round**: Technical Interview

1.  **Problem**: (Same as Shubhanshi's Q3) Given an array, you can perform an operation `k` times: divide an element by 2 and take its ceiling. Find the minimum sum of the array.
    * **Solution**: Use a max heap.
2.  **Problem**: A grasshopper can make jumps according to a given `jumps` array. Find the minimum starting stair number (`>=1`) so that after making all jumps, its position is always on a valid stair (i.e., stair number `> 0`).
    * **Solution**: Binary search on the answer (the starting stair).
3.  **Discussion**: Questions about a research internship and projects.

---

### **Deepanshi Verma**
* **Interviewer**: Shashank Mishra
* **Round**: Technical Interview

1.  **Discussion**: Project discussion about an Android project.
2.  **OOPs**: Polymorphism, Inheritance, Function Overloading, Function Overriding, Constructors, and the Singleton Class concept.
3.  **Problem**: Reverse a linked list.
4.  **Problem**: How many queens can be placed safely on an `N x N` chessboard? (N-Queens problem).
    * **Follow-up**: Discussed the method (backtracking) and data structures used in the recursive implementation.

---

### **Swathi Keerthana Muda**
* **Interviewer**: Rohit
* **Round**: Technical Interview
* **Discussion**: Introduction and Project (10 mins)

1.  **Problem**: Given an array and an integer `k`, group all numbers less than `k` together. Find the minimum number of swaps required.
    * **Example**: `arr[] = {2, 1, 5, 6, 3}`, `k = 3`. Answer: 1 (swap 5 with 1).
    * **Solution**: Use the **Sliding Window** technique. The size of the window is the total count of elements less than `k`.
    * **Complexity**: `O(n)` Time, `O(1)` Space.

---

### **Sanjana Kumari**
* **Interviewer**: Himanshu Jindal
* **Round**: Technical Interview 1
* **Discussion**: Intro & project (10 min), NoSQL vs. MySQL, Function vs. Operator Overloading, Multi-threading in C++.

1.  **Problem**: Given a number `N` as a string, find the smallest number greater than `N` that can be formed using the same set of digits. If no such number exists, return "Not possible".
    * **Solution**: This is the [Next Permutation](https://leetcode.com/problems/next-permutation/description/) problem.

---

### **Devansh Srivastava**
* **Interviewer**: Kaustubh Vats
* **Round**: Technical Interview

1.  **Problem**: Remove all duplicate elements from a sorted linked list.
    * **Solution**: Use a two-pointer approach or a single pointer checking `current->next`.
2.  **Problem**: Design a system to handle requests for unique IDs. It should support adding an element (allocating the smallest available ID), and freeing an ID upon removal.
    * **Example**: `Add 15` (ID 1), `Add 20` (ID 2), `Smallest` (returns 3), `Remove 20` (ID 2 is free), `Smallest` (returns 2).
    * **Solution**: Use a map to track used IDs and a min-priority-queue or set to store freed IDs.
3.  **OOPs**: Virtual functions, virtual destructors, access modifiers, and smart pointers.

---

### **Shambhavi Verma**
* **Interviewer**: Vaishali
* **Round**: Technical Interview

1.  **Problem**: **Three Sum**. Find all unique triplets in an array that sum to a target value.
    * **Solution**: Sort the array, then use a two-pointer approach inside a loop.
2.  **Problem**: **Four Sum**. Find all unique quadruplets that sum to a target.
    * **Solution**: An efficient approach uses a map to store the sum of previous pairs.
    * **Follow-ups**:
        * When to use an ordered (`std::map`) vs. unordered (`std::unordered_map`) map?
        * Explain the difference in their time complexities and internal implementation (BST vs. Hash Table).
        * What is hashing? How does a hash table work?
3.  **OOPs**: Fundamentals (Pillars of OOPs), Inheritance, and its use cases.

---

### **Sonalika Chandra**
* **Interviewer**: Shobhit Mittal
* **Round**: Technical Interview

1.  **Problem**: **Unbounded Knapsack** type DP problem. You have a certain amount of money and `m` stores. Each store sells a bundle of notebooks (`bundleQuantities[i]`) for a certain cost (`bundleCosts[i]`). Find the maximum number of notebooks you can buy. You can buy any number of bundles from any store.
    * **Solution**: Started with recursion, then memoized to a DP solution.
2.  **OOPs & OS**:
    * Implement a `Calculator` class with a method that takes two arguments and returns the result.
    * Basics of Multithreading.

---

### **Krishna Purwar**
* **Interviewer**: Prakhar
* **Round**: Technical Interview

1.  **Problem**: Given an array of integers and a `threshold` value, find the minimum integer divisor such that the sum of the divisions (ceiling of `arr[i]/divisor`) for each element is less than or equal to the `threshold`.
    * **Solution**: Binary search on the answer (the divisor).
2.  **Problem**: Shuffle an array such that no element remains in its original index.
    * **Solution**: A variation of the Fisher-Yates shuffle. For each index `i`, generate a random index `j` in the range `[i+1, n-1]` and swap `arr[i]` with `arr[j]`. (Note: This doesn't guarantee the condition but is a common shuffling approach).
3.  **Problem**: (Same as Shubhanshi's Q2) Given two sorted arrays and a value `x`, find the pair whose sum is closest to `x`.

---

### **Kavya**
* **Interviewer**: Amanpreet
* **Round**: Technical Interview

1.  **Problem**: (Same as Divyam's Q2) A grasshopper jumps on a staircase. Given an array of jumps (positive for up, negative for down), find the lowest possible starting stair number (`>=1`) so that the grasshopper never lands on a stair numbered less than 1.
2.  **Problem**: You have `n` chocolates with given weights. Every day, you can pick one chocolate, eat half of it (`floor(weight/2)`), and put it back. Find the minimum possible total weight after `d` days.
    * **Solution**: Use a max heap (priority queue or `std::multiset`). On each day, pick the heaviest chocolate, halve its weight, and put it back.
3.  **Theory**: General OOPs and SQL questions.

---

### **Haswanthi**
* **Interviewer**: Shrey Trivedi
* **Round**: Technical Interview

1.  **Discussion (10 min)**: Introduction, project discussion (from GitHub, not resume), and C++ basics (`const int`, pointers, OOPs).
2.  **Problem (20 min)**: A number is represented by a linked list (e.g., `1->9->8` is 198). Increment the number by one and return the head of the new list (e.g., `1->9->9`).
    * **Solution**: Use recursion to traverse to the end, then handle the carry-over while backtracking.
3.  **Problem (30 min)**: Check if a given binary tree is a **Binary Search Tree (BST)**.
    * **Link**: [Check for BST](https://www.geeksforgeeks.org/a-program-to-check-if-a-binary-tree-is-bst-or-not/)
    * **Solution**: Provided multiple methods, but the interviewer focused on the **inorder traversal** approach. An inorder traversal of a valid BST produces a sorted sequence.

---

### **Suruchi Kumari**
* **Interviewer**: Shashank Goel
* **Round**: Technical Interview 1
* **Discussion**: Project Discussion (10 mins)

1.  **Problem**: [Next Greater Element](https://www.geeksforgeeks.org/next-greater-element/).
    * **Solution**: Use a stack.
2.  **Problem**: Given an array of strings, group all anagrams together. The relative order of the first occurrence of each anagram group should be maintained.
    * **Example**: `["cat", "dog", "tac", "god", "act"]` -> `["cat", "tac", "act", "dog", "god"]`
    * **Solution**: Use a hash map where the key is the sorted version of a string and the value is a list of its anagrams.

---

### **Shruti Kumari**
* **Round**: Technical Interview 1
* **Discussion**: Intro and Project (15 mins), C++ fundamentals.

1.  **Theory**: Define Stack, Queue, Linked List, Graph, and Trie. What are the differences between a Linked List and a Queue?
2.  **Problem**: You are given a paragraph containing some web links. Design a system to store these links. If a link is queried, return it if present; otherwise, return -1.
    * **Follow-up**: Which data structure would you use, and what would be its time complexity? (A hash set or Trie would be suitable).
