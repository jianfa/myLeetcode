
# 问题：

977. Squares of a Sorted Array 

# Problem: [977 Squares of a Sorted Array ](<https://leetcode.com/problems/squares-of-a-sorted-array/> )

## 描述 Description
> ### Given an array of integers `A` sorted in non-decreasing order, return an array of the squares of each number, also in sorted non-decreasing order. ### 

## 例子 Example

> ```
> Input: [-4,-1,0,3,10]
> Output: [0,1,9,16,100]
> 
> Input: [-7,-3,2,3,11]
> Output: [4,9,9,49,121]
> ```

## 分析 Analysis

核心思想：
> 思路1：compute the squares and sort it
>> 时间复杂度：O(nlogn)
>> 空间复杂度：O(n)

> 思路2：two pointers
>> 时间复杂度：O(n)
>> 空间复杂度：O(n)

## 定义 Definition

### Python


```python
class Solution:
    def sortedSquares(self, A: List[int]) -> List[int]:
        # solution 1: squared and then sort
        # Time complexity: O(NlogN)
        # Space complexity: O(N)
        # input control
        if A == None:
            return None
        # square the value
        A = [num * num for num in A]
        # sort the list
        return sorted(A)
    
 class Solution:
    def sortedSquares(self, A: List[int]) -> List[int]:
        # solution 2: two pointers
        # step 1: find the position of first non-negative value
        # step 2: from center to two endings, compare two values
        # Time complexity: O(N)
        # Space complexity: O(N)
        
        # input control
        if A == None:
            return None
        # find the first non-negative value
        r = 0 # left and right pointers
        while r < len(A) and A[r] < 0:
            r += 1
        l = r - 1

        # traverse from center to two endings
        res = []
        while r < len(A) and l >= 0:
            if -A[l] > A[r]:
                res.append(A[r]**2)
                r += 1
            else:
                res.append(A[l]**2)
                l -= 1
        while r < len(A):
                res.append(A[r]**2)
                r += 1
        while l >= 0:
                res.append(A[l]**2)
                l -= 1
        return res
class Solution:
    def sortedSquares(self, A: List[int]) -> List[int]:
        # solution 3, two pointers, from two ending to center
        # Time complexity: O(N)
        # Space complexity: O(N)
        if A == None:
            return None
        l,r = 0,len(A)-1
        res = [0] * len(A)
        p  = r
        A = [x**2 for x in A]
        while l <= r:
            if A[l] > A[r]:
                res[p] = A[l]
                l += 1
                p -= 1
            else:
                res[p] = A[r]
                r -= 1
                p -= 1
        return res
        
        
```

### C++

```c++

```

### Java

```java

```

## 解决方案 Solution

### 1.

> 时间复杂度：O()
> 空间复杂度：O()

### Python


```python

```

### C++

```c++

```

### Java

```java

```

### 2.

> 时间复杂度：O()
> 空间复杂度：O()

### Python


```python

```

### C++

```c++

```

### Java

```Java

```

## 总结

### 1.看到这个问题，我最初是怎么思考的？我是怎么做的？遇到了哪些问题？
> 

### 2.别人是怎么思考的？别人是怎么做的？
> 

### 3.与他的做法相比，我有哪些可以提升的地方？
> 


```python

```
