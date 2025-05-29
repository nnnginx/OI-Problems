## 题目描述
You are given an array of $n$ positive integers $a_1$, $a_2$, $\ldots$, $a_n$, as well as a positive integer $k$. You need to divide the array into $k$ non-empty subsequences such that each element of the array belongs to exactly one subsequence. A subsequence is a sequence that can be obtained from another sequence by deleting some elements without changing the order of the remaining elements.

Let the $i$-th subsequence contain elements with indices $j_1 < \ldots < j_l$. The $\textit{value}$ of this subsequence is defined as the maximum value of $a_{j_m} + m$ for all $m$ from $1$ to $l$.

The $\textit{cost}$ of dividing the array into $k$ subsequences is the sum of the $\textit{values}$ of these subsequences.

Find the maximum $\textit{cost}$ of the division.

## 输入格式
The first line contains two positive integers $n$ and $k$ ($1 \leq k \leq n \leq 500\,000$) --- the size of the array and the number of subsequences to divide it into.

The second line contains $n$ positive integers $a_1$, $a_2$, $\ldots$, $a_n$ ($1 \leq a_i \leq 10^9$) --- the elements of the array.

## 输出格式
Output the maximum $\textit{cost}$ of dividing the given array into $k$ non-empty subsequences.

```input1
5 3
3 7 10 1 2
```

```output1
24
```

## 提示
**Note**

In the sample test, the array can be divided into $[3, 10]$, $[7]$, $[1, 2]$. Then the answer will be $(10 + 2) + (7 + 1) + (2 + 2) = 12 + 8 + 4 = 24$.

**Scoring**

The tests for this problem consist of six groups. Points for each group are given only if all tests of the group and all tests of the required groups are passed.

| Group | Points | Additional Constraints: $n$ | Additional Constraints: $k$ | Required Groups | Comment                        |
| :---- | :----- | :---------------------------- | :---------------------------- | :-------------- | :----------------------------- |
| 0     | 0      | --                            | --                            | --              | Examples.                      |
| 1     | 14     | $n \le 8$                   | --                            | 0               |                                |
| 2     | 19     | --                            | $k = 2$                     | --              |                                |
| 3     | 17     | --                            | --                            | --              | $a_{i+1} \leq a_i$           |
| 4     | 21     | --                            | --                            | --              | $a_{i+1} \geq a_i - 1$       |
| 5     | 15     | $n \leq 1000$               | --                            | 0, 1            |                                |
| 6     | 14     | --                            | --                            | 0 -- 5          |                                |

