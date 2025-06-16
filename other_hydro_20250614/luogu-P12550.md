## 题目描述
Given a string $s$ consisting of characters $\texttt{A}$, $\texttt{B}$, and $\texttt{C}$.

In one operation, you are allowed to choose two **adjacent** elements of the string $s_is_{i+1}$ that are in the following order: $\texttt{AB}$, $\texttt{BC}$, or $\texttt{CA}$, and swap them.

Find the maximum number of consecutive operations that can be performed on the string $s$.

In this problem, each test contains several sets of input data. You need to solve the problem independently for each such set.

## 输入格式
The first line contains one integer $T$ $(1\le T\le 10^5)$ --- the number of sets of input data. The description of the input data sets follows.

In the first line of each input data set, there is one integer $n$ $(1 \le n \le 10^6)$ --- the length of the string $s$.

In the second line of each input data set, there is a string $s$ of length $n$, consisting of characters $\texttt{A}$, $\texttt{B}$, and $\texttt{C}$.

It is guaranteed that the sum of $n$ across all input data sets of a single test does not exceed $10^6$.

## 输出格式
For each set of input data, output on a separate line one integer --- the maximum number of consecutive operations that can be performed on the string $s$.

```input1
2
5
ABCCA
19
CCAABBBABBAAABBCCAA
```

```output1
3
28
```

## 提示
In the first set of input data from the first example, no more than $3$ consecutive operations can be performed on the string $\texttt{ABCCA}$. One example of how $3$ consecutive operations can be performed is $[\texttt{ABCCA} \rightarrow \texttt{BACCA}, \texttt{BACCA} \rightarrow \texttt{BACAC}, \texttt{BACAC} \rightarrow \texttt{BAACC}]$.

### Scoring

Let $K$ be the sum of $n$ over all input data sets of one test.

- ($2$ points): the answer is equal to $0$ or $1$;
- ($3$ points): $n \le 3$;
- ($5$ points): $s_i \ne \texttt{C}$ for $1 \le i \le n$;
- ($5$ points): $s$ has the form $\texttt{AA}\ldots \texttt{AABB}\ldots \texttt{BBCC}\ldots \texttt{CC}$ (that is, $x \cdot \texttt{A} + y \cdot \texttt{B} + z \cdot \texttt{C}$ for certain positive $x$, $y$, $z$);
- ($9$ points): $s_is_{i+1} \ne \texttt{CA}$ for $1 \le i < n$;
- ($10$ points): $T = 1$, $n \le 12$;
- ($8$ points): $n \le 12$;
- ($28$ points): $K \le 2000$;
- ($30$ points): without additional constraints.

