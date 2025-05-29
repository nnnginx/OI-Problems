## 题目描述

给定正整数数列 $a_1\sim a_N$。

有 $Q$ 个操作：

- $\texttt{?}$ $k$：查询 $\displaystyle \sum_{1\le i\le N-k+1} \max(a_i,a_{i+1},\ldots,a_{i+k-1})$；
- $\texttt{+}$ $k$：令 $a_k\gets a_{k}+1$。


## 输入格式

>
>
> $N$ $Q$\
> $a_1$ $a_2$ $\ldots$ $a_N$\
> $\mathrm{op}_1$ $k_1$\
> $\vdots\quad\vdots$\
> $\mathrm{op}_Q$ $k_Q$

其中，$\mathrm{op}_i\in \{\texttt{?},\texttt{+}\}$，$1\le k_i\le N$，描述一次操作。

## 输出格式

对每个 $\texttt{?}$ 操作输出一行一个正整数，表示答案。

```input1
6 5
1 7 2 3 5 4
+ 1
? 2
? 3
+ 5
? 3
```

```output1
27
24
26
```

```input2
10 4
1 2 2 1 3 2 1 3 2 2
? 4
? 5
+ 5
? 4
```

```output2
20
18
24
```

## 提示

### 数据范围

- $1\le N\le 5\times 10^5$；
- $0\le Q\le 5\times 10^5$；
- $1\le A_i\le 10^9$；
- $\mathrm{op}_i\in \{\texttt{?},\texttt{+}\}$；
- $1\le k_i\le N$；
- 所有输入的数均为整数。

### 子任务

Subtask 0 为样例。

| 子任务编号 | $N,Q\le$ | 特殊性质 | 得分 |
| :-: | :-: | :-: | :-: |
| $1$ | $7\, 000$ | $-$ | $13$ |
| $2$ | $5\times 10^5$ | $\text{A}$ | $16$ |
| $3$ | $5\times 10^5$ | $\text{B}$ | $23$ |
| $4$ | $5\times 10^5$ | $\text{C}$ | $10$ |
| $5$ | $10^5$ | $-$ | $20$ |
| $6$ | $5\times 10^5$ | $-$ | $18$ |

- 特殊性质 $\text{A}$：$\mathrm{op}_i\neq\texttt{+}$；
- 特殊性质 $\text{B}$：$a_i\le 10$；
- 特殊性质 $\text{C}$：对于所有 $\texttt{?}$ $k_i$ 操作，$k_i$ 均相等。


