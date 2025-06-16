## 题目描述
Given a sequence $a_1, a_2, \ldots, a_n$.

You are going to select zero or more elements of $a$ so that: if you select $a_i$, then in any interval of length $i$ (formally, in $a[j, j + i - 1]$ for any $1 \le j \le n - i + 1$) you can select at most $2$ elements.

Calculate the maximal sum of the elements you select.

## 输入格式
The first line contains an integer $n$ ($2 \leq n \leq 10^5$).

The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^9 \leq a_i \leq 10^9$).

## 输出格式
Output a single integer denoting the answer.

```input1
4
1 4 3 2

```

```output1
7

```

```input2
3
-10 -10 -10

```

```output2
0
```

## 提示
**Source**: The 2022 ICPC Asia Xi'an Regional Contest Problem J.

**Author**: JohnVictor.

