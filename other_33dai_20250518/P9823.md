## 题目描述
Once upon a time, there was a witch named Geor Autumn, who set off on a journey across the world. Along the way, she would meet all kinds of people, from a country full of ICPC competitors to a horse in love with dota---but with each meeting, Geor would become a small part of their story, and her own world would get a little bit bigger.

Geor just arrived at the state of Shu where people love poems. A poem is a permutation $(a_1,\ldots, a_n)$ of $[n]$. ($(a_1,\ldots, a_n)$ is a permutation of $[n]$ means that each $a_i$ is an integer in $[1,n]$ and that $a_1,\ldots, a_n$ are distinct.) One poem is $\textit{good}$ if for all integer $i$ satisfying $i> k$ and $i\le n$, $a_i>\min(a_{i-k}, \ldots, a_{i-1})$. Here $\min(a_{i-k}, \ldots, a_{i-1})$ denotes the minimum value among $a_{i-k}, \ldots, a_{i-1}$.

Help Geor calculate how many good poems there are, given $n$ and $k$. To avoid huge numbers, output the answer modulo $998244353$.

## 输入格式
The first line contains two integers $n$ and $k$ separated by a single space ($1\le n\le 10^7$, $1\le k\le 10^7$).

## 输出格式
Output only one integer in one line---the number of good poems modulo $998244353$.

## 题目大意
### 题意简述
给定 $1 \le k \le n$，我们规定满足以下性质的 $1 \sim n$ 的排列称之为“好排列”：

$\forall k<i \le n,~a_i > \min{a_{i-k},a_{i-k+1},...,a_{i-1}}$

求好排列的个数。对 $998244353$ 取模。
### 输入格式
一行，两个整数 $n,k$。
### 输出格式
一行，为好排列的个数对 $998244353$ 取模的值。

```input1
1 1
```

```output1
1
```

```input2
2 3
```

```output2
2
```

```input3
3 2
```

```output3
4
```

```input4
4 2
```

```output4
10
```

