## 题目描述
Following up on a journal article about increasing milk production, Bessie has become the Baric Bovine by studying atmospheric pressure in order to curry favor with Farmer John.

She takes N (1 <= N <= 100) measurements conveniently named M\_1 through M\_N during the day (1 <= M\_i <= 1,000,000); these measurements are numbered in the order in which Bessie observed them.

In order to characterize the day's atmospheric pressure readings, she is interested in finding a subset of the measurements (given by the K (1 <= K <= N) indices s\_j where 1 <= s\_1 < s\_2 < ... < s\_K <= N) that accurately reflects the entire set, i.e., limits the error as described below.

In any subset of measurements, an error is incurred for each

measurement (1) before the first member of the subset, (2) between two consecutive measurements in the subset, and (3) after the last member of the subset. The total error value for a given set of s\_j values is the sum of each of the individual errors.

Specifically, for all measurements whose index i is not one of the s\_j values:

```cpp
* if i is less than s_1, then the sample error is: 
2 * | M_i - M_(s_1) | 
* if i is between s_j and s_(j+1), then the sample error is 
| 2 * M_i - Sum(s_j, s_(j+1)) | 
where Sum(x, y) = M_x + M_y; 
* if i is greater than s_K, then the sample error is 
2 * | M_i - M_(s_K) | 
Given a maximum error value E (1 <= E <= 1,000,000), determine the size of the smallest subset of measurements that produces an error of at most E. 
```


## 输入格式
\* Line 1: Two space-separated integers: N and E

\* Lines 2..N+1: Line i+1 contains a single integer: M\_i


## 输出格式
\* Line 1: Two space-separated integers: the size of the smallest subset of measurements that produces an error of at most E and the least possible error for the subset of that size.


## 题目大意
## 题目描述

为了研究农场的气候，Bessie 帮助农夫 John 做了  $N$ 次气压测量并按顺序记录了结果  $M_1 \cdots M_n$。Bessie 想找出一部分测量结果来总结一整天的气压分布。她想用  $K(1 \leq K \leq N)$ 个数  $s_j (1 \leq s_1 < s_2 < \cdots < s_K \leq N)$ 来概括所有测量结果。她想限制如下的误差: 对于任何测量结果子集，每一个非此子集中的结果都会产生误差。总误差是所有测量结果的误差之和。更明确地说，对于每一个和所有  $s_j$ 都不同的  $i$：

- 如果  $i$ 小于  $s_1$, 误差是： $2 \times | M_i - M_{(s_1)} |$；
- 如果  $i$ 在  $s_j$ 和  $s_{(j+1)}$ 之间，误差是： $| 2 \times M_i - \operatorname{Sum}(s_j, s_{(j+1)}) |$。注： $\operatorname{Sum}(x, y) = M_x + M_y$  ( $M_x$ 和  $M_y$ 之和)；
- 如果  $i$ 大于  $s_K$ ,误差为： $2 \times | M_i - M_{(s_K)} |$ 给出最大允许的误差  $E$，找出最小的一部分结果使得误差最多为  $E$。

## 输入格式

- 第  $1$ 行：两个用空格分开的正整数  $N$ 和  $E$。

- 第  $2\cdots N+1$ 行：第  $i+1$ 行包含单独的一个正整数  $M_i$。

## 输出格式

- 第  $1$ 行：两个用空格分开的整数，分别代表着最小的使得误差小于等于  $E$ 的测量结果子集元素的数量和其能达到的最小误差值。

## 说明/提示

### 数据范围

对于所有数据， $1 \leq N \leq 100$， $1 \leq M_i \leq 1,000,000$， $1 \leq E \leq 1,000,000$。

### 样例说明

Bessie 做了 4 次测量，最大允许的误差是 20。测量的结果分别为 10，3，20 和 40。

选择第二次和第四次测量结果是最佳的，误差为 17。第一个结果的误差为  $2\times|10-3|=14$，第三个的为  $|2\times20-(3+40)|=3$。

```input1
4 20 
10 
3 
20 
40 

```

```output1
2 17 

```

## 提示
Bessie takes four measurements; the maximum error is 20. The

measurements are, in sequence: 10, 3, 20, and 40.


Choosing the second and fourth measurements is the best option, giving an error of 17. The first term's error is 2\*|10-3| = 14; the third term's error is |2\*20 - (3+40)| = 3. 

