## 题目描述
**This is a problem with graders.**

For an array of positive integers $b$ of length $m$, we define $f(b)$ as follows:

- Let initially a variable $x$ be equal to $0$;
- For one **coin**, it is allowed to increase the value of $x$ by $1$;
- For one **coin**, it is allowed to choose an element of the array $b_i$ ($1\le i\le m$) and replace it with $(b_i \oplus x)$, where $\oplus$ denotes the operation of  **bitwise exclusive OR**;
- $f(b)$ equals the minimum number of coins needed to make all elements of the array $b$ simultaneously equal to zero.

The **bitwise exclusive OR** of non-negative integers $a$ and $b$ $(a \oplus b)$ equals a non-negative integer, in which in the binary representation, there is a one at a certain position only if in the binary representations of $a$ and $b$ at this position there are different values. For example, $3_{10} \oplus 5_{10} = 0011_{2} \oplus 0101_{2} = 0110_{2} = 6_{10}$.

An array of positive integers $a$ of length $n$ and $q$ queries of the form $l$, $r$ are given. For each query, it is necessary to find $f([a_l,a_{l+1},\ldots,a_r])$. 

You need to implement the following functions:

```
void init(integer n, array of integers a)
```

- $n$ --- an integer representing the length of the array;
- $a$ --- an array of integers of length $n$;
- this function does not return anything.

```
integer ask(integer l, integer r)
```

- $l$ --- an integer representing the left boundary of the query;
- $r$ --- an integer representing the right boundary of the query;
- this function returns an integer --- $f([a_l,a_{l+1},\ldots,a_r])$.

```
array of integers askAll(integer q, array of integers l, array of integers r)
```

- $q$ --- an integer representing the number of queries;
- $l$ --- an array of integers of length $q$; $l_i$ represents the left boundary of the $i$-th query;
- $r$ --- an array of integers of length $q$; $r_i$ represents the right boundary of the $i$-th query;
- this function returns an array of integers; the $i$-th number should be equal to the answer to the $i$-th query.

## 输入格式
The first line contains three integers $n$, $q$, and $t$ ($1 \leq n, q \leq 2 \cdot 10^5$; $1 \leq t \leq 2$) --- the number of numbers, the number of queries, and the format of the queries, respectively.

The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \leq a_i < 2^{60}$) --- the elements of the array $a$.

The next $q$ lines contain two integers $l$ and $r$ ($1 \leq l \leq r \leq n$) --- the parameters of the $i$-th query.

The function $\tt{init}$ will be called exactly once.

If $t=1$, then the function $\tt{askAll}$ with all queries will be called exactly once. If $t=2$, then the function $\tt{ask}$ will be called exactly $q$ times.

## 输出格式
The grader will output $q$ integers in separate lines --- the answers to the queries.

```input1
7 6 1
5 4 3 5 7 7 7
1 4
4 7
3 7
1 7
2 6
1 1
```

```output1
9
11
12
14
12
6
```

```input2
7 6 2
5 4 3 5 7 7 7
1 4
4 7
3 7
1 7
2 6
1 1
```

```output2
9
11
12
14
12
6
```

## 提示
### Scoring

- ($3$ points): $t=1$, $a_i=a_1$ for $1\le i\le n$;
- ($8$ points): $t=1$, $a_i \neq a_j$ for $i \neq j$;
- ($3$ points): $t=1$, $2^m+n \le a_i<2^{m+1}$ for some natural $m$;
- ($9$ points): $t=1$, $a_i \le a_{i+1}$ for $1 \le i < n$;
- ($10$ points): $t=1$, $n, q \le 1000$;
- ($11$ points): $t=1$, $l_i=1$ and $r_i=i$ for $1\le i\le q$.
- ($10$ points): $t=1$, $n, q \le 50000$;
- ($25$ points): $t=1$;
- ($9$ points): $t=2$, $n, q \le 10^5$;
- ($12$ points): $t=2$.

