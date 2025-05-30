## 题目描述
Paimon just invents a new sorting algorithm which looks much like $\textit{bubble sort}$, with a few differences. It accepts a $1$-indexed sequence $A$ of length $n$ and sorts it. Its pseudo-code is shown below.

```cpp
// The Sorting Algorithm
SORT(A)
  for i from 1 to n // n is the number of elements if A
    for j from 1 to n
      if a[i] < a[j] // a[i] is the i-th element in A
        Swap a[i] and a[j]
```


If you don't believe this piece of algorithm can sort a sequence it will also be your task to prove it. Anyway here comes the question:

Given an integer sequence $A = a_1, a_2, \cdots, a_n$ of length $n$, for each of its prefix $A_k$ of length $k$ (that is, for each $1 \le k \le n$, consider the subsequence $A_k = a_1, a_2, \cdots, a_k$), count the number of swaps performed if we call $\text{SORT}(A_k)$.

## 输入格式
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains an integer $n$ ($1 \le n \le 10^5$) indicating the length of the sequence.

The second line contains $n$ integers $a_1, a_2, \cdots, a_n$ ($1 \le a_i \le n$) indicating the given sequence.

It's guaranteed that the sum of $n$ of all test cases will not exceed $10^6$.

## 输出格式
For each test case output one line containing $n$ integers $s_1, s_2, \cdots, s_n$ separated by a space, where $s_i$ is the number of swaps performed if we call $\text{SORT}(A_i)$.

Please, DO NOT output extra spaces at the end of each line or your solution may be considered incorrect!

## 题目大意
给出一个排序算法（用伪代码表示）：

```cpp
// 排序算法
SORT(A)
  for i from 1 to n // n 是序列 A 的元素个数
    for j from 1 to n
      if a[i] < a[j] // a[i] 是序列 A 的第 i 个元素
        Swap a[i] and a[j]

```

请你算出对于一个序列 $A=a_1,a_2,\cdots,a_n$ 的所有前缀 $A_k=a_1,a_2,\cdots,a_k$（$1\le k\le n$），$\operatorname{SORT}(A_k)$ 中的交换（Swap）操作将会被执行几次。

```input1
3
5
2 3 2 1 5
3
1 2 3
1
1

```

```output1
0 2 3 5 7
0 2 4
0

```

