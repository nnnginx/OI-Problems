## 题目描述

Farmer John is building a brand new, $n$-story barn, with the help of his $k$ cows. To build it as quickly as possible, he needs your help to figure out how to allocate work among the cows.Each cow must be assigned to work on exactly one specific floor out of the $n$ total floors in the barn, and each floor must have at least one cow assigned to it. The iith floor requires $a_i$ units of total work, and each cow completes one unit of work per hour, so if $c$ cows work on floor $i$, it will be completed in $\dfrac{a_i}{c}$ units of time. For safety reasons, floor $i$ must be completed before construction can begin on floor $i+1$.

Please compute the minimum total time in which the barn can be completed, if the cows are allocated to work on floors in an optimal fashion. 

Output this number rounded to the nearest integer; it is guaranteed that the solution will be more than $0.1$ from the boundary between two integers.

## 输入格式

The first line of input contains $n$ and $k$.

The next $n$ lines contain $a_1\cdots a_n$, each a positive integer.

## 输出格式

Please output the minimum time required to build the barn, rounded to the nearest integer.

```input1
2 5
10
4
```

```output1
5
```

## 数据规模与约定

对于 $100\%$ 的数据，满足 $1\le n\le k\le 10^{12}$，$1\le n \le 10^5$，$1\le a_i \le 10^{12}$。

## 题目来源

Platinum