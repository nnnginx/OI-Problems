## 题目描述
You are given an array of integers $a$ of length $n$.

Determine whether there exists a permutation of its elements $b$ such that for every $2\leq i \leq n-1$, the condition $b_{i-1} + b_{i+1} \ge 2\cdot b_i$ holds.

In this problem, each test contains several sets of input data. You need to solve the problem independently for each such set.

## 输入格式
The first line contains a single integer $T$ $(1\le T\le 10^5)$ --- the number of sets of input data. The description of the input data sets follows.

In the first line of each input data set, there is a single integer $n$ $(3\le n\le 3\cdot 10^5)$ --- the length of the array $a$.

In the second line of each input data set, there are $n$ integers $a_1, a_2, \ldots, a_n$ $(0\le a_i\le 10^9)$ --- the elements of the array $a$.

It is guaranteed that the sum of $n$ across all input data sets of a single test does not exceed $3\cdot 10^5$.

## 输出格式
For each set of input data, output on a separate line $\tt{YES}$, if the desired permutation exists, and $\tt{NO}$ otherwise.

```input1
10
4
0 3 4 6
4
5 4 1 4
8
1 4 4 8 6 10 10 4
7
2 1 5 1 9 4 6
6
7 1 6 10 2 3
7
6 6 10 2 5 3 8
4
9 9 1 5
4
8 4 3 4
7
1 2 1 6 4 2 9
7
3 9 7 5 9 10 10
```

```output1
YES
NO
NO
YES
YES
NO
YES
YES
YES
NO
```

## 提示
In the first set of input data from the first example, the permutations of the array $[0, 3, 4, 6]$ that satisfy the described condition are $[4, 0, 3, 6]$ and $[6, 3, 0, 4]$.

### Scoring

Let $S$ be the sum $n$ over all input data sets of one test.

- ($3$ points): $n = 4$;
- ($4$ points): $T = 1$, $n \le 7$;
- ($7$ points): $T = 1$, $n \le 15$;
- ($5$ points): if some desired permutation exists, then there exists such a desired permutation for which $b_1 \ge b_2$ and $b_2 \le b_3$;
- ($17$ points): $S \le 50$;
- ($10$ points): $S \le 400$;
- ($13$ points): $S \le 2000$;
- ($9$ points): $S \le 8000$;
- ($18$ points): $a_i \le 10^6$ for $1 \le i \le n$;
- ($14$ points): without additional restrictions.

