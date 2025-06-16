## 题目描述
We call a non-empty sequence of positive integers *strange* if the sum of its elements is a prime number.

You are given an array $a$ of length $n$, **consisting of prime numbers**. You are also given an integer $k$.

Split the array $a$ into $k$ **non-empty** subsequences$^1$ such that each element of the array $a$ belongs to exactly one of them, and the number of *strange* subsequences among the formed ones is minimized.

In this problem, each test contains several sets of input data. You need to solve the problem independently for each such set.

**Note that there is no block "without additional constraints" in this problem.**

## 输入格式
The first line contains one integer $T$ $(1\le T\le 10^5)$ --- the number of sets of input data. The description of the input data sets follows.

In the first line of each input data set, two integers $n$, $k$ $(1 \le k \le n \le 10^5)$ are given --- the length of the array $a$ and the number of subsequences into which it needs to be split.

In the second line of each input data set, $n$ prime numbers $a_1, a_2, \ldots, a_n$ $(2\le a_i\le 10^5, a_i\le a_{i+1})$ are given --- the elements of the array $a$.

It is guaranteed that the sum of $n$ across all input data sets of one test does not exceed $10^5$.

## 输出格式
For each set of input data, output the optimal partition in the following format:

- In the first line, output one integer $m$ --- the number of *strange* subsequences among the formed ones;
- In each of the next $k$ lines, output integers $s_i$ and $b_1, b_2, \ldots, b_{s_i}$ $(1\le s_i\le n)$ --- the number of elements in the corresponding subsequence of the partition and the elements themselves.

Subsequences and their elements may be output in any order.

If there are multiple correct answers, any of them is allowed.

```input1
4
3 1
5 5 13
4 2
2 3 5 7
5 3
3 3 5 5 13
6 5
2 2 2 3 3 3
```

```output1
1
3 13 5 5
0
2 2 7
2 3 5
1
1 13
2 3 3
2 5 5
4
1 2
1 2
1 2
1 3
2 3 3
```

## 提示
$^1$ A sequence $c$ is called a subsequence of an array $b$ if it is possible to remove a certain number of elements from the array $b$ (possibly zero) so that the sequence $c$ is formed.

### Scoring

- ($2$ points): $T \leq 20$, $k=1$;
- ($5$ points): $n \leq 4$, $a_i \leq 10^4$ for all $1\le i\le n$;
- ($8$ points): $T \leq 20$, $n \leq 10$, $a_i \leq 10^4$ for all $1\le i\le n$;
- ($4$ points): $n$ --- even, $a_i > 2$ for all $1\le i\le n$;
- ($18$ points): $n$ --- odd, $a_i > 2$ for all $1\le i\le n$;
- ($10$ points): $2\cdot k \ge n + 1$;
- ($29$ points): $n$ --- even;
- ($24$ points): $n$ --- odd.

