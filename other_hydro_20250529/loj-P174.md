## Description

Given two sequences $a_0, \dots, a_n, b_0, \dots, b_m$ and a positive integer $M$. Calculate an integer sequence $c_0, \dots, c_{n+m}$, satisfying:

$$
c_k = \sum_{i=\max(k-m,0)}^{\min(k,n)} \binom k i a_i b_{k-i} \bmod M
$$

Here $\binom k i = \frac{k!}{i!(k-i)!}$ denotes the binomial coefficient.


## Input Format

The first line consists of integer $n, m, M$.

The second line consists of $a_0,\dots,a_n$.

The third line consists of $b_0,\dots,b_m$.

## Output Format

Print one line, containing $c_0,\dots,c_{n+m}$.



```input1
2 5 114
5 1 4
1 9 1 9 8 10
```

```output1
5 46 27 42 100 108 84 42
```

## Limits

For $10\%$ of the test cases, it's guaranteed that $n,m\le 10^3$.

For another $20\%$, $M$ is a prime.

For another $20\%$, $M$ is a power of $2$.

For $100\%$ of the test cases, it's guaranteed that $0\le n, m\le 10^5, 2\le M\le 10^9, 0\le a_i, b_j < M$.

