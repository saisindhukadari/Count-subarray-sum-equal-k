# Count Subarray Sum Equals K (Brute Force)

## Problem Statement

Given an integer array and an integer `k`, find the total number of contiguous subarrays whose sum is equal to `k`.

## Approach

This solution uses the **Brute Force** approach.

For every index in the array:

* Consider it as the starting point of a subarray.
* Extend the subarray one element at a time.
* Maintain a running sum while extending the subarray.
* If the running sum becomes equal to `k`, increment the count.
* Repeat the process for all starting indices.

## Algorithm

1. Read the input array and the value of `k`.
2. Initialize a variable to store the answer.
3. Traverse the array using the first loop as the starting index.
4. Reset the running sum for every new starting index.
5. Extend the subarray using the second loop.
6. Add the current element to the running sum.
7. If the running sum equals `k`, increment the count.
8. Print the total count.

## Pattern Used

* Brute Force
* Nested Loops
* Running Sum

## Time Complexity

* **O(n²)**

## Space Complexity

* **O(1)**

## Notes

* Every possible subarray is considered exactly once.
* The running sum avoids recalculating the sum of each subarray from scratch.
* This is the standard brute-force solution and is useful for understanding the problem before learning the optimal prefix sum + hashing approach.
