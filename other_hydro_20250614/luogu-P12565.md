## 题目描述
You are given two integers, $a$ and $b$. You concatenate all the numbers in the range $[a, b]$ in an order that produces the largest possible number, $x$.

You are given $q$ queries of the form: $k$ --- what is the $k$-th digit of $x$?

The digits of $x$ are $0$-indexed, starting with the most significant one. 

It is guaranteed that the length of $x$ will be at least $k + 1$.

## 输入格式
The first line contains two integers $a$ and $b$ ($0 < a \leq b \leq 10^{17}$).

The second line contains one integer $q$ ($1 \leq q \leq 5 \cdot 10^4$). 

The third line contains $q$ integers $k_1, k_2, \dots, k_q$ ($0 \leq k_i \leq 2 \cdot 10^{18}$), representing the queries. It is guaranteed that all answers exist.

## 输出格式
The only line of the output should contain a string of length $q$, where the $i$-th character will be the answer to the $i$-th query.

```input1
8 13
4
0 3 8 9
```

```output1
9310
```

## 提示
- ($4$ points): $b - a \leq 7$;
- ($4$ points): $len(a) = len(b)$;
- ($10$ points): $b - a \leq 100000$
- ($33$ points): $q \leq 30$;
- ($23$ points): $q \leq 1\,000$;
- ($16$ points): $q \leq 10\,000$;
- ($10$ points): no further restrictions.

