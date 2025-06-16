## Description

Byteasar intends to throw up a party. Naturally, he would like it to be a success. Furthermore, Byteasar is quite certain that to make it so it suffices if all invited guests know each other. He is currently trying to come up with a list of his friends he would like to invite. Byteasar has friends, where is divisible by  $3$. Fortunately, most of Byteasar's friends know one another. Furthermore, Byteasar recalls that he once attended a party where there were $\dfrac 23n$ of his friends, and where everyone knew everyone else. Unfortunately, Byteasar does not quite remember anything else from that party... In particular, he has no idea which of his friends attended it. Byteasar does not feel obliged to throw a huge party, but he would like to invite at least $\dfrac n3$ of his friends. He has no idea how to choose them, so he asks you for help.

## Input

In the first line of the standard input two integers, $n$ and $m$, are given, separated by a single space. These denote the number of Byteasar's friends and the number of pairs of his friends who know each other, respectively.

Byteasar's friends are numbered from $1$ to $n$.

Each of the following $m$ lines holds two integers separated by a single space.

The numbers in line no. $i+1$ (for $i=1,2,...,m$) are $a_i$ and $b_i$, separated by a single space, which denote that the persons $a_i$ and $b_i$ know each other. Every pair of numbers appears at most once on the input.

## Output

In the first and only line of the standard output your program should print $\dfrac n3$ numbers, separated by single spaces, in increasing order. These number should specify the numbers of Byteasar's friends whom he should invite to the party. As there are multiple solutions, pick one arbitrarily.

```input1
6 10
2 5
1 4
1 5
2 4
1 3
4 5
4 6
3 5
3 4
3 6
```

```output1
2 4
```

## Constraints

For $100\%$ data, $3\le n\le 3000$, $\dfrac{\dfrac 23n\left(\dfrac 23n-1\right)}{2}\leq m\leq \dfrac{n(n-1)}2$, $1\le a_i < b_i\le n$.

## Source

Thanks to Object022 & suhang.

