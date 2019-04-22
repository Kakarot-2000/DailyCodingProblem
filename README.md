# DailyCodingProblem
https://www.dailycodingproblem.com/

[TOC]


## 1 [Eazy]
This problem was recently asked by Google.  

Given a list of numbers and a number k, return whether any two numbers from the list add up to k. 
For example, given [10, 15, 3, 7] and k of 17, return true since 10 + 7 is 17. 

Bonus: Can you do this in one pass?  

HINT. https://leetcode.com/problems/two-sum/

## 2 [Hard]
This problem was asked by Uber.  

Given an array of integers, return a new array such that each element at index i of the new array is the product of all the numbers in the original array except the one at i.  

For example, if our input was [1, 2, 3, 4, 5], the expected output would be [120, 60, 40, 30, 24]. If our input was [3, 2, 1], the expected output would be [2, 3, 6].

HINT. https://leetcode.com/problems/product-of-array-except-self/

## 3 [Medium]
This problem was asked by Google.

Given the root to a binary tree, implement `serialize(root)`, which serializes the tree into a string, and `deserialize(s)`, which deserializes the string back into the tree.

For example, given the following `Node` class

```
class Node:
    def __init__(self, val, left=None, right=None):
        self.val = val
        self.left = left
        self.right = right
```

The following test should pass:

```
node = Node('root', Node('left', Node('left.left')), Node('right'))
assert deserialize(serialize(node)).left.left.val == 'left.left'
```

HINT. https://leetcode.com/problems/serialize-and-deserialize-binary-tree/

If <u>val</u> could be any string that contains spaces or other special characters, some extra job should be done to encode and decode it, e.g. how the C do with character '/'. 

## 4 [Hard]

This problem was asked by Stripe.

Given an array of integers, find the first missing positive integer in linear time and constant space. In other words, find the lowest positive integer that does not exist in the array. The array can contain duplicates and negative numbers as well.

For example, the input `[3, 4, -1, 1]` should give `2`. The input `[1, 2, 0]`should give `3`.

You can modify the input array in-place.

HINT. <https://leetcode.com/problems/first-missing-positive/>



## 5 [medium]

This problem was asked by Jane Street.

`cons(a, b)` constructs a pair, and `car(pair)` and `cdr(pair)` returns the first and last element of that pair. For example, `car(cons(3, 4))` returns `3`, and `cdr(cons(3, 4))` returns `4`.

Given this implementation of cons:

```
def cons(a, b):
    def pair(f):
        return f(a, b)
    return pair
```

Implement `car` and `cdr`.

HINT1. <https://galaiko.rocks/posts/2018-07-06/>

HINT2. <https://stackoverflow.com/questions/52481607/dont-understand-the-inner-function-in-python>