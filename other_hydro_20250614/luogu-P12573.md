## 题目描述
Given an integer $m$, an array $a$ of non-negative integers of length $n$, and $q$ queries of the form $l_i$, $r_i$. All elements of array $a$ are less than $2^m$.

Let us define the function $f_i(x) = \min_{j \in [l_i, r_i]} (a_j \oplus x)$, where $\oplus$ denotes the bitwise exclusive OR operation. For each query, you need to find the value $\max_{x \in \{0, 1, \ldots, 2^m-1\}} f_i(x)$.

Bitwise exclusive OR of non-negative integers $a$ and $b$ $(a \oplus b)$ equals a non-negative integer that has a 1 in a certain position in its binary representation if and only if the binary representations of $a$ and $b$ have different values in that position. For example, $3_{10} \oplus 5_{10} = 0011_{2} \oplus 0101_{2} = 0110_{2} = 6_{10}$.

## 输入格式
The first line contains three integers $n$, $q$, $m$ ($1 \le n \le 10^5$, $1 \le q \le 5 \cdot 10^5$, $1 \le m \le 50$), representing the length of the array, the number of queries, and the limit on the elements of the array, respectively.

The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i < 2^m$), representing the elements of the array.

The following $q$ lines each contain two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le n$), representing the parameters of the $i$-th query.

## 输出格式
For each $i$-th query, output a single integer on a separate line --- the value of $\max_{x \in \{0, 1, \ldots, 2^m-1\}} f_i(x)$.

```input1
5 5 3
1 3 2 7 1
1 5
2 3
3 4
1 3
1 1
```

```output1
3
6
3
5
7
```

## 提示
The first query. 

$f_1(0)=\min(1 \oplus 0, 3 \oplus 0, 2 \oplus 0, 7 \oplus 0, 1 \oplus 0)=\min(1, 3, 2, 7, 1)=1$

$f_1(1)=\min(1 \oplus 1, 3 \oplus 1, 2 \oplus 1, 7 \oplus 1, 1 \oplus 1)=\min(0, 2, 3, 6, 0)=0$

$f_1(2)=\min(1 \oplus 2, 3 \oplus 2, 2 \oplus 2, 7 \oplus 2, 1 \oplus 2)=\min(3, 1, 0, 5, 3)=0$

$f_1(3)=\min(1 \oplus 3, 3 \oplus 3, 2 \oplus 3, 7 \oplus 3, 1 \oplus 3)=\min(2, 0, 1, 4, 2)=0$

$f_1(4)=\min(1 \oplus 4, 3 \oplus 4, 2 \oplus 4, 7 \oplus 4, 1 \oplus 4)=\min(5, 7, 6, 3, 5)=3$

$f_1(5)=\min(1 \oplus 5, 3 \oplus 5, 2 \oplus 5, 7 \oplus 5, 1 \oplus 5)=\min(4, 6, 7, 2, 4)=2$

$f_1(6)=\min(1 \oplus 6, 3 \oplus 6, 2 \oplus 6, 7 \oplus 6, 1 \oplus 6)=\min(7, 5, 4, 1, 7)=1$

$f_1(7)=\min(1 \oplus 7, 3 \oplus 7, 2 \oplus 7, 7 \oplus 7, 1 \oplus 7)=\min(6, 4, 5, 0, 6)=0$

The answer to this query is equal to $\max_{x \in \{0, 1, \ldots, 2^3-1\}} f_1(x) = \max(1, 0, 0, 0, 3, 2, 1, 0) = 3$.

### Scoring

- ($4$ points): $n \le 100$, $q \le 100$, $m \le 10$;
- ($17$ points): $q=1$, $l_1=1$, $r_1=n$;
- ($16$ points): $q \le 2 \cdot 10^5$; $a_i \le a_{i+1}$ for $1 \le i < n$;
- ($17$ points): $n\le 10^4$, $q \le 10^4$;
- ($26$ points): $n \le 5 \cdot 10^4$, $m \le 30$;
- ($20$ points): no additional constraints.

