# Cheetcode Special Problems

## [Valid Palindrome](https://leetcode.com/problems/valid-palindrome/)
```
Given a string s, determine if it is a palindrome, 
considering only alphanumeric characters and ignoring cases.

Example 1
  Input: s = "A man, a plan, a canal: Panama"
  Output: true
  Explanation: "amanaplanacanalpanama" is a palindrome.

Example 2
  Input: s = "race a car"
  Output: false
  Explanation: "raceacar" is not a palindrome.

Constraints
  1 <= s.length <= 2 * 105
  s consists only of printable ASCII characters.
```

```javasript
```


## [Valid Palindrome II](https://leetcode.com/problems/valid-palindrome-ii/)
```
Given a non-empty string s, you may delete at most one character. 
Judge whether you can make it a palindrome.

Example 1
  Input: "aba"
  Output: True

Example 2
  Input: "abca"
  Output: True
  Explanation: You could delete the character 'c'.
  Note: The string will only contain lowercase characters a-z. The maximum length of the string is 50000.
```

```javasript
```


## [Kth Largest Element in an Array](https://leetcode.com/problems/kth-largest-element-in-an-array/)
```
Given an integer array nums and an integer k, return the kth largest element in the array.

Note that it is the kth largest element in the sorted order, not the kth distinct element.

Example 1
  Input: nums = [3,2,1,5,6,4], k = 2
  Output: 5

Example 2
  Input: nums = [3,2,3,1,2,4,5,5,6], k = 4
  Output: 4
 
Constraints
  1 <= k <= nums.length <= 104
  -104 <= nums[i] <= 104
```

```javasript
```


## [Serialize and Deserialize Binary Tree](https://leetcode.com/problems/serialize-and-deserialize-binary-tree/)
```
Serialization is the process of converting a data structure or object into a sequence of bits so that it can be stored in a file or memory buffer, or transmitted across a network connection link to be reconstructed later in the same or another computer environment.

Design an algorithm to serialize and deserialize a binary tree. There 
is no restriction on how your serialization/deserialization algorithm 
should work. You just need to ensure that a binary tree can be serialized to a string and this string can be deserialized to the original tree structure.

Clarification: The input/output format is the same as how LeetCode serializes a 
binary tree. You do not necessarily need to follow this format, so please be 
creative and come up with different approaches yourself.

Example 1
          1
         /   \
       2      3
             / \
       	  4   5
       	  
  Input: root = [1,2,3,null,null,4,5]
  Output: [1,2,3,null,null,4,5]

Example 2
  Input: root = []
  Output: []

Example 3
  Input: root = [1]
  Output: [1]

Example 4
  Input: root = [1,2]
  Output: [1,2]
 
Constraints
  The number of nodes in the tree is in the range [0, 104].
  -1000 <= Node.val <= 1000
```

```javasript
```


## [Add Binary](https://leetcode.com/problems/add-binary/)
```
Given two binary strings a and b, return their sum as a binary string.

Example 1
  Input: a = "11", b = "1"
  Output: "100"

Example 2
  Input: a = "1010", b = "1011"
  Output: "10101"
 
Constraints
  1 <= a.length, b.length <= 104
  a and b consist only of '0' or '1' characters.
  Each string does not contain leading zeros except for the zero itself.
```

```javasript
```

## [Given read4 ii call multiple times](https://leetcode.com/problems/read-n-characters-given-read4-ii-call-multiple-times/)
```
Given a file and assume that you can only read the file using a given method read4, implement a method read to read n characters. Your method read may be called multiple times.

** Look at leetcode problem to learn what read4 is **

Note
  - Consider that you cannot manipulate the file directly. The file is only accessible for read4 but not for read.
  - The read function may be called multiple times.
  - Please remember to RESET your class variables declared in Solution, as static/class variables are persisted across multiple test cases. Please see here for more details.
  - You may assume the destination buffer array, buf, is guaranteed to have enough space for storing n characters.
  - It is guaranteed that in a given test case the same buffer buf is called by read.
 
Example 1
  Input: file = "abc", queries = [1,2,1]
  Output: [1,2,0]
  Explanation: The test case represents the following scenario:
    File file("abc");
    Solution sol;
    sol.read(buf, 1); // After calling your read method, buf should contain "a". We read a total of 1 character from the file, so return 1.
    sol.read(buf, 2); // Now buf should contain "bc". We read a total of 2 characters from the file, so return 2.
    sol.read(buf, 1); // We have reached the end of file, no more characters can be read. So return 0.
    Assume buf is allocated and guaranteed to have enough space for storing all characters from the file.

Example 2
  Input: file = "abc", queries = [4,1]
  Output: [3,0]
  Explanation: The test case represents the following scenario:
    File file("abc");
    Solution sol;
    sol.read(buf, 4); // After calling your read method, buf should contain "abc". We read a total of 3 characters from the file, so return 3.
    sol.read(buf, 1); // We have reached the end of file, no more characters can be read. So return 0.
 

Constraints
  1 <= file.length <= 500
  file consist of English letters and digits.
  1 <= queries.length <= 10
  1 <= queries[i] <= 500
```

```javasript
```


## [Decode String](https://leetcode.com/problems/decode-string/)
```
Given an encoded string, return its decoded string.

The encoding rule is: k[encoded_string], where the encoded_string inside 
the square brackets is being repeated exactly k times. Note that k is 
guaranteed to be a positive integer.

You may assume that the input string is always valid; No extra white spaces,
 square brackets are well-formed, etc.

Furthermore, you may assume that the original data does not contain any digits and 
that digits are only for those repeat numbers, k. For example, 
there won't be input like 3a or 2[4].

Example 1
  Input: s = "3[a]2[bc]"
  Output: "aaabcbc"

Example 2
  Input: s = "3[a2[c]]"
  Output: "accaccacc"

Example 3
  Input: s = "2[abc]3[cd]ef"
  Output: "abcabccdcdcdef"

Example 4
  Input: s = "abc3[cd]xyz"
  Output: "abccdcdcdxyz"
 
Constraints
  1 <= s.length <= 30
  s consists of lowercase English letters, digits, and square brackets '[]'.
  s is guaranteed to be a valid input.
  All the integers in s are in the range [1, 300].
```

```javasript
```

## [Shortest Path in a Grid with Obstacles Elimination](https://leetcode.com/problems/shortest-path-in-a-grid-with-obstacles-elimination/)
```
You are given an m x n integer matrix grid where each cell is either 0 (empty) or 1 (obstacle). You can move up, down, left, or right from and to an empty cell in one step.

Return the minimum number of steps to walk from the upper left corner (0, 0) to the lower right corner (m - 1, n - 1) given that you can eliminate at most k obstacles. If it is not possible to find such walk return -1.

Example 1:



Input: grid = [[0,0,0],[1,1,0],[0,0,0],[0,1,1],[0,0,0]], k = 1
Output: 6
Explanation: 
The shortest path without eliminating any obstacle is 10.
The shortest path with one obstacle elimination at position (3,2) is 6. Such path is (0,0) -> (0,1) -> (0,2) -> (1,2) -> (2,2) -> (3,2) -> (4,2).

```

```javasript
```

## [K Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin/)
```
```

```javasript
```

## [Dot Product of Two Sparse Vector](https://leetcode.com/problems/dot-product-of-two-sparse-vectors/)
```
```

```javasript
```

## [Sparse Matrix Multiplication](https://leetcode.com/problems/sparse-matrix-multiplication/)
```
```

```javasript
```

## [Divide Two Integers](https://leetcode.com/problems/divide-two-integers/)
```
```

```javasript
```

## [LRU Cache](https://leetcode.com/problems/lru-cache/)
```
```

```javasript
```

## [Monotonic Array](https://leetcode.com/problems/monotonic-array/)
```
```

```javasript
```

## [Candy Crush](https://leetcode.com/problems/candy-crush/)
```
```

```javasript
```

## [Letter Combinations of a Phone Number](https://leetcode.com/problems/letter-combinations-of-a-phone-number/)
```
```

```javasript
```

## [asteroid-collision](https://leetcode.com/problems/asteroid-collision/)
```
```

```javasript
```

## [time-based-key-value-store](https://leetcode.com/problems/time-based-key-value-store/)
```
```

```javasript
```

## [friend-circles]()
```
```

```javasript
```

## [Number of Provinces (optional?)](https://leetcode.com/problems/number-of-provinces/)
```
```

```javasript
```

## [valid-parentheses](https://leetcode.com/problems/valid-parentheses/)
```
```

```javasript
```

## [product-of-array-except-self](https://leetcode.com/problems/product-of-array-except-self/)
```
```

```javasript
```

## [string-compression](https://leetcode.com/problems/string-compression/)
```
```

```javasript
```

## [design-hit-counter](https://leetcode.com/discuss/interview-question/178662/Design-a-Hit-Counter/) [Google Onsite Version](https://leetcode.com/discuss/interview-question/615505/Google-or-Onsite-or-Design-Hit-Counter)
```
```

```javasript
```

## [logger-rate-limiter](https://leetcode.com/problems/logger-rate-limiter/)
```
```

```javasript
```

## [number-of-distinct-islands](https://leetcode.com/problems/number-of-distinct-islands/)
```
```

```javasript
```

## [design-hashmap](https://leetcode.com/problems/design-hashmap/)
```
```

```javasript
```

## [Game of Life](https://leetcode.com/problems/game-of-life/)
```
```

```javasript
```

## [Basic Calculator II](https://leetcode.com/problems/basic-calculator-ii/)
```
```

```javasript
```
