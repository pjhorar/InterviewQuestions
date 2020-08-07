


## 1. Single Number III

Given an array of numbers nums, in which exactly two elements appear only once and all the other elements appear exactly twice. Find the two elements that appear only once.

> Input:  [1,2,1,3,2,5]

> Output: [3,5]

## 2. Spiral Matrix

Given a matrix of m x n elements (m rows, n columns), return all elements of the matrix in spiral order.

> Input:
[
 [ 1, 2, 3 ],
 [ 4, 5, 6 ],
 [ 7, 8, 9 ]
]

> Output: [1,2,3,6,9,8,7,4,5]

## 3. Add Digits

Given a non-negative integer num, repeatedly add all its digits until the result has only one digit.

> Input: 38

> Output: 2 

> Explanation: The process is like: 3 + 8 = 11, 1 + 1 = 2. 
             Since 2 has only one digit, return it.
             
## 4. Maximum Width of Binary Tree

Given a binary tree, write a function to get the maximum width of the given tree. The maximum width of a tree is the maximum width among all levels.

The width of one level is defined as the length between the end-nodes (the leftmost and right most non-null nodes in the level, where the null nodes between the end-nodes are also counted into the length calculation.

It is guaranteed that the answer will in the range of 32-bit signed integer.

> Input: 

           1
         /   \
        3     2
       / \     \  
      5   3     9 
      
> Output: 4

> Explanation: The maximum width existing in the third level with the length 4 (5,3,null,9).

## 5. Min Stack

Design a stack that supports push, pop, top, and retrieving the minimum element in constant time.

  * push(x) -- Push element x onto stack.
  * pop() -- Removes the element on top of the stack.
  * top() -- Get the top element.
  * getMin() -- Retrieve the minimum element in the stack.
   
> Input
["MinStack","push","push","push","getMin","pop","top","getMin"]
[[],[-2],[0],[-3],[],[],[],[]]

> Output
[null,null,null,null,-3,null,0,-2]

> 
Explanation
MinStack minStack = new MinStack();
minStack.push(-2);
minStack.push(0);
minStack.push(-3);
minStack.getMin(); // return -3
minStack.pop();
minStack.top();    // return 0
minStack.getMin(); // return -2

## 6. Populating Next Right Pointers in Each Node

You are given a perfect binary tree where all leaves are on the same level, and every parent has two children. The binary tree has the following definition:
```C++
struct Node {
  int val;
  Node *left;
  Node *right;
  Node *next;
}
```
Populate each next pointer to point to its next right node. If there is no next right node, the next pointer should be set to NULL.

Initially, all next pointers are set to NULL.

 

Follow up:

   You may only use constant extra space.
   Recursive approach is fine, you may assume implicit stack space does not count as extra space for this problem.
   
Example 1:

![Images of Binary Tree](https://assets.leetcode.com/uploads/2019/02/14/116_sample.png)

> Input: root = [1,2,3,4,5,6,7]

> Output: [1,#,2,3,#,4,5,6,7,#]

> Explanation: Given the above perfect binary tree (Figure A), your function should populate each next pointer to point to its next right node, just like in Figure B. The serialized output is in level order as connected by the next pointers, with '#' signifying the end of each level.

## . Minimum Add to Make Parentheses Valid

Given a string S of '(' and ')' parentheses, we add the minimum number of parentheses ( '(' or ')', and in any positions ) so that the resulting parentheses string is valid.

Formally, a parentheses string is valid if and only if:

   * It is the empty string, or
   * It can be written as AB (A concatenated with B), where A and B are valid strings, or
   * It can be written as (A), where A is a valid string.

Given a parentheses string, return the minimum number of parentheses we must add to make the resulting string valid.

> Example 1:
 Input: "())"
 Output: 1

> Example 2:
 Input: "((("
 Output: 3

> Example 3:
 Input: "()"
 Output: 0

> Example 4:
 Input: "()))(("
 Output: 4

## 7. Divide Array in Sets of K Consecutive Numbers

Given an array of integers nums and a positive integer k, find whether it's possible to divide this array into sets of k consecutive numbers
Return True if its possible otherwise return False.

> Example 1:

> Input: nums = [1,2,3,3,4,4,5,6], k = 4

> Output: true

> Explanation: Array can be divided into [1,2,3,4] and [3,4,5,6].

Constraints 

   * 1 <= nums.length <= 10^5
   * 1 <= nums[i] <= 10^9
   * 1 <= k <= nums.length
   
## 8. Maximum Sum Circular Subarray

Given a circular array C of integers represented by A, find the maximum possible sum of a non-empty subarray of C.

Here, a circular array means the end of the array connects to the beginning of the array.  (Formally, C[i] = A[i] when 0 <= i < A.length, and C[i+A.length] = C[i] when i >= 0.)

Also, a subarray may only include each element of the fixed buffer A at most once.  (Formally, for a subarray C[i], C[i+1], ..., C[j], there does not exist i <= k1, k2 <= j with k1 % A.length = k2 % A.length.)

Note:

   * -30000 <= A[i] <= 30000
   * 1 <= A.length <= 30000
   
Example 

> Input: [3,-1,2,-1]

> Output: 4

> Explanation: Subarray [2,-1,3] has maximum sum 2 + (-1) + 3 = 4


## 9. Count Square Submatrices with All Ones

Given a m * n matrix of ones and zeros, return how many square submatrices have all ones.

> Example 

> Input: matrix =
[
  [0,1,1,1],
  [1,1,1,1],
  [0,1,1,1]
]

> Output: 15

> Explanation: 
  There are 10 squares of side 1.
  There are 4 squares of side 2.
  There is  1 square of side 3.
  Total number of squares = 10 + 4 + 1 = 15.
