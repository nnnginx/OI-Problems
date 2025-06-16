## 题目描述
We call an array of integers $d_1, d_2, \ldots, d_m$ *good* if its length is equal to $0$, or for any $1\le i\le m$, both values $\sum\limits_{j=1}^{i} d_j$ and $\sum\limits_{j=i}^{m} d_j$ are non-negative. Here, $\sum\limits_{j=l}^{r} d_j$ denotes $d_l+d_{l+1}+\ldots+d_{r}$.

We define the *beauty* of the array as the length of its longest *good* subsequence$^1$.

You are given an array $a$ of length $n$, which **consists of numbers $-1$ and $1$**.

You need to perform $q$ queries. The queries are of two types:

- replace the element $a_p$ with $-a_p$, where $p$ --- the parameter of the query;
- find the *beauty* of the array consisting of elements $[a_{l},a_{l+1},\ldots,a_r]$, where $(l, r)$ --- the parameters of the query.

## 输入格式
In the first line, two integers $n$, $q$ are given $(1\le n, q\le 5 \cdot 10^5)$ --- the length of the array $a$ and the number of queries, respectively.

In the second line, $n$ integers $a_1, a_2, \ldots, a_n$ $(a_i \in \{-1, 1\})$ are given --- the elements of the array $a$.

In the next $q$ lines, the description of the queries is given. The first of the numbers $type_i$ $(1 \le type_i \le 2)$ denotes the type of the query. Queries of the first type are given in the format $\texttt{1 p}$ $(1 \le p \le n)$, and queries of the second type are given in the format $\texttt{2 l r}$ $(1 \le l \le r \le n)$.

## 输出格式
For each query of the second type, output one integer in a separate line --- the *beauty* of the corresponding array.

```input1
5 4
1 1 1 -1 1
2 1 5
1 3
2 1 4
2 2 5
```

```output1
5
2
3
```

```input2
4 4
1 1 1 -1
2 1 2
2 2 4
2 3 3
2 3 4
```

```output2
2
2
1
1
```

## 提示
$^1$ An array $c$ is called a subsequence of an array $b$ if it is possible to remove a certain number of elements from the array $b$ (possibly zero) so that the array $c$ is formed. The empty array is a subsequence of any array.

### Scoring

- ($2$ points): $a_i = (-1)^{i+1}$ for $1 \le i \le n$, and there are no type one queries;
- ($7$ points): $n \le 16$, and there are no type one queries;
- ($21$ points): $n, q \le 100$;
- ($20$ points): $n, q \le 3000$;
- ($27$ points): $n, q \leq 2 \cdot 10^5$, and there are no type one queries;
- ($14$ points): $n, q \leq 2 \cdot 10^5$;
- ($9$ points): no additional restrictions.

