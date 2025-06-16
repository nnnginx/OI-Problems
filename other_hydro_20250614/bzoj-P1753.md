## 题目描述

FJ is surveying his herd to find the most average cow. He wants to know how much milk this 'median' cow gives: half of the cows give as much or more than the median; half give as much or less.

Given an odd number of cows $N$ and their milk output, find the median amount of milk given such that at least half the cows give the same amount of milk or more and at least half give the same or less.

输入 $N$ 个数，输出升序排列后中间那个数。 

## 输入格式

* Line $1$: A single integer $N$.
* Lines $2\sim N+1$: Each line contains a single integer that is the milk output of one cow.

## 输出格式

* Line $1$: A single integer that is the median milk output.

```input1
5
2
4
1
3
5
```

```output1
3
```

## 样例说明

Five cows with milk outputs of $1\sim 5$.

$1$ and $2$ are below $3$; $4$ and $5$ are above $3$.

## 数据规模与约定 

对于 $100\%$ 的数据：$1 \leq N < 10^4$，$1\leq$ 产奶量 $\leq 10^6$。

## 题目来源

Usaco2005 qua