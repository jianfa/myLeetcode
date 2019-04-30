# 高效刷 LeetCode

## `Binary Search 二分查找`
特点：逐渐缩小范围，每一次可以删掉一部分（不一定要一半），难点在于分析该怎么移动使得删除后原来的属性没有变化。
适用类型：1. 已经排好序，2.找峰值。

Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[704. Binary Search](https://github.com/jianfa/myLeetcode/blob/master/code/704.md) | Binary Search 模板 | √ | 
[162. Find Peak Element](https://github.com/jianfa/myLeetcode/blob/master/code/162.md) | 找峰值 | √ | 
[4. Median of two ssorted array](https://github.com/jianfa/myLeetcode/blob/master/code/4.md) | 找Kth值 | √ | 
[34. Find First and Last Position of Element in Sorted Array](https://github.com/jianfa/myLeetcode/blob/master/code/34.md) | 套用704的模板就行 | √ | 
[74. Search a 2D Matrix](https://github.com/jianfa/myLeetcode/blob/master/code/74.md) | 套用704的模板就行 | √ |
[153. Find Minimum in Rotated Array](https://github.com/jianfa/myLeetcode/blob/master/code/153.md) | 套用704的模板就行 | √ |
[81. Search in Rotated Array II](https://github.com/jianfa/myLeetcode/blob/master/code/81.md) | 套用704的模板就行,注意mid = left= right的情况 | √ |
[302. Smallest rectangel enclosing black pixels](https://github.com/jianfa/myLeetcode/blob/master/code/302.md) | 用binary search分别找四个边界 | √ |


## `Breadth first search`

适合找minimum depth 或者step类型的题目

BFS 三步骤：  
1. find start node  
2. update level node list  
3. the ending condition 


Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[102. Binary Tree Level Traversal](https://github.com/jianfa/myLeetcode/blob/master/code/102.md) | BFS模板 | √ | 
[310. Minimum Height Tree](https://github.com/jianfa/myLeetcode/blob/master/code/310.md) | BFS bottom-up的应用 | √ | 
[542. 01 Matrix](https://github.com/jianfa/myLeetcode/blob/master/code/542.md) | BFS bottom-up的应用 | √ | 
[127. Word Ladder](https://github.com/jianfa/myLeetcode/blob/master/code/127.md) | BFS top-down| √ | 
[934. Shortest Bridge](https://github.com/jianfa/myLeetcode/blob/master/code/934.md) | 两遍BFS top-down| √ | 
[407. Trapping Rain Water II](https://github.com/jianfa/myLeetcode/blob/master/code/407.md) | minimum heap + bottom-up BFS| √ | 
[743. Network Delay Time](https://github.com/jianfa/myLeetcode/blob/master/code/743.md) | Graph+Dijkstra+heap | √ | 

## `Dynamic programming`
DP的本质是减少循环和重复计算次数，用空间换取时间。
这些问题可以用到DP：  
  1. 找最大/最小  
  2. Yes/No  
  3. Count  

用DP解题，分四个步骤  
1. state function  
2. initialization  
3. update function  
4. final result  
 
  DP问题的最大难点在于对state function的构造，以及如何update。  
  
Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[120. Triangle](https://github.com/jianfa/myLeetcode/blob/master/code/120.md) | 标准动规题 | √ |  


## `Search -BFS/DFS`
有递归和非递归两大类，又分为pre-order, in-order, post-order三类

Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[529. Minesweeper](https://github.com/jianfa/myLeetcode/blob/master/code/529.md) | DFS | √ | 
[530. Minimum Absolute Difference in BST](https://github.com/jianfa/myLeetcode/blob/master/code/530.md) |  BST,in-order traversal, non-recursive traversal | √ | 
[897. Increasing Order Search Tree](https://github.com/jianfa/myLeetcode/blob/master/code/897.md) | DFS,用generator | √ | 


## `Array`

Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[977. Squares of a Sorted Array]( <https://github.com/jianfa/myLeetcode/blob/master/code/977_Squares_of_a_sorted_array.md>  ) |  | √ |


## `Stack 栈`

Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[85. Largest Rectangle in Histogram](https://github.com/jianfa/myLeetcode/blob/master/code/85.md) | 巧妙使用栈解决问题的范例 | √ | 
[155. Min Stack] | 最小值栈 | √ | 

## `Linked List 链表`

Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[2. Add Two Numbers] | 求两数和 | √ | 
[21. Merge Two Sorted Lists] | 合并两个有序链表 | √ | 
[23. Merge k Sorted Lists] | 合并K个有序链表 | √ | √ 
[86. Partition List 链表划分] | 链表划分 | √ | √ 
[108. Convert Sorted Array to Binary Search Tree] | 转换有序数组为二叉搜索树 | √ | 
[109. Convert Sorted List to Binary Search Tree] | 转换有序链表为二叉搜索树 | √ | 
[141. Linked List Cycle] | 判断链表中是否有环 | √ | 
[160. Intersection of Two Linked Lists] | 两个链表的交点 | √ | 
[206. Reverse Linked List] | 反转链表 | √ | 
[234. Palindrome Linked List] | 回文链表 | √ | 
[237. Delete Node in a Linked List] | 删除链表任意节点 | √ | √ 

## `String 字符串`

Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[3. Longest Substring Without Repeating Characters] | 无重复字符的最长子串 | √ | 
[5. Longest Palindromic Substring] | 最长回文子串 | √ | 
[6. ZigZag Conversion] | 字符串锯齿形变换 | √ | 
[8. String to Integer (atoi)] | 字符串转换为整数 | √ | 
[9. Palindrome Number] | 回文数 | √ | 
[13. Roman to Integer] | 罗马字符转换为整数 | √ | 
[14. Longest Common Prefix] | 最长公共前缀 | √ | 
[17. Letter Combinations of a Phone Number] | 电话号码按键包含字符的所有组合 | √ | 
[28. Implement strStr()] | B 在 A 中第一次出现的索引 | √ | 
[38. Count and Say] | Count and Say | √ | √ 
[46. Permutations] | 字符串全排列 | √ | 
[125. Valid Palindrome] | 回文串判断（字符串中包含标点空格） | √ | 
[171. Excel Sheet Column Number]) | Excel 表格栏编号 | √ | 
[242. Valid Anagram] | 有效字谜 | √ | 
[344. Reverse String] | 反转字符串 | √ | 
[383. Ransom Note] | A 是否可由 B 构造 | √ | 
[412. Fizz Buzz] | Fizz Buzz | √ | 
[680. Valid Palindrome II] | 字符串中至多删除一个字符后是否可以构成回文串 | √ | 
[647. Palindromic Substrings] | 回文子串个数 | √ | 

## `Dynamic Programming 动态规划`

Problem | Remark | Python 
:------- | :----- | :----: 
[10. Regular Expression Matching] | 正则表达式匹配 | √ 
[70. Climbing Stairs] | 台阶问题 | √ 
[198. House Robber] | 盗贼盗窃 | √ 




## `Tree 树`

Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[124. Binary Tree Maximum Path Sum](https://github.com/jianfa/myLeetcode/blob/master/code/124.md) |divide and conquer | √ |
[101. Symmetric Tree] | 对称树 | √ | 
[104. Maximum Depth of Binary Tree] | 二叉树最大深度 | √ | 

## `Hash Table 哈希表`

Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[136. Single Number] | 单数 | √ | 
[202. Happy Number] | 快乐数（重复计算所有位数字平方和，最终是否得到1） | √ | 
[217. Contains Duplicate] | 包含重复数 | √ | 
[350. Intersection of Two Arrays II] | 两个数组的交集 | √ | 
[387. First Unique Character in a String] | 第一个不重复的字符 | √ | 

## `Math 数学`

Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[172. Factorial Trailing Zeroes] | 阶乘尾随零点 | √ | √ 
[204. Count Primes] | 小于 n 的素数 | √ | 
[326. Power of Three] | 判断一个数是否是3 的幂 | √ | 

## `Bit Manipulation 位运算`

Problem | Remark | Python | C++ 
:------- | :----- | :----: | :----: 
[190. Reverse Bits] | 反转位 | √ | 
[191. Number of 1 Bits] | 二进制中1的个数 | √ | 
[371. Sum of Two Integers] | 两个整数的和 | √ | √ 

[算法笔记模板](https://github.com/jianfa/myLeetcode/blob/master/template.md)

The template is credited to [Decalogue](https://github.com/Decalogue/AlgorithmMap)

 Copyright © 2019 Jianfa. All Rights Reserved.`


