## 题目描述
Lately, Slavko’s been studying sequences of natural numbers. He finds a sequence
interesting if the greatest common divisor of all the elements from the sequence is greater
than 1.

Yesterday, he found a sequence consisting of N natural numbers in his garage. Since he
was really bored, he decided to keep himself occupied by asking simple queries. Each query
can be one of the two types:

1. Change the value at position X in the sequence to V.

2. Determine the number of interesting contiguous subarrays contained in the interval
[L, R] of the sequence.


## 输入格式
The first line of input contains the numbers N and Q (1 ≤ N, Q ≤ $10^5$
), representing the
number of elements in the sequence and the number of queries, respectively.

The following line contains N natural numbers $A_i$
(1 ≤ $A_i$ ≤ $10^9$
) that represent the numbers in
the initial sequence.

Each of the following Q lines contains a query of the following form:

 - The first number in the line can be 1 or 2 and represents the type of the query.
 - If the query is of type 1, two numbers follow, X (1 ≤ X ≤ N) and V (1 ≤ V ≤ $10^9$
) from
the task.
 - If the query is of type 2, two numbers follow, L and R (1 ≤ L ≤ R ≤ N) that represent
the left and right interval boundary.


## 输出格式
For each query of type 2, output the number of interesting contiguous subarrays from the
task.


## 题目大意
最近，斯科拉夫一直在研究自然数的序列。如果序列中所有数的最大公约数大于1，他会认为序列很有趣。昨天，他在车库里发现了一个由N个自然数组成的序列。由于他真的很无聊，他决定通过做两种操作使自己有事做 1:将序列中位置X的值更改为V    2：确定序列的区间[L，R]中包含的有趣的连续子阵列的数量


```input1
5 1
8 4 3 9 1
2 2 5

```

```output1
4
```

```input2
5 3
2 3 6 4 1
2 1 4
1 3 1
2 3 5

```

```output2
6
1

```

```input3
4 3
2 2 2 2
2 1 4
1 2 3
2 1 4

```

```output3
10
5
```

## 提示
**Clarification​ ​of​ ​the​ ​first​ ​test​ ​case:**

The interval from the $2_{nd}$ to the $5_{th}$ position consists of numbers (4, 3, 9, 1). In it, the following are
interesting contiguous subarrays (denoted with square brackets):
**[4]**​ 3 9 1, 4 **[3]​** ​9 1, 4 3 **[9]**​ 1, 4 **[3​ ​9]​** 1

