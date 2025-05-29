## ��Ŀ����
There are $n$ contestants and they take part in $m$ contests. You are given the ranklist of each contest. The ranklist of the $k$-th contest is a sequence $a_k$, indicating that the $a_{k, i}$-th contestant's rank is $i$.

SolarPea and PolarSea are two of the $n$ contestants. SolarPea wants to prove that he is stronger than PolarSea.

Define $x$ is $l$-stronger than $y$, if and only if there exists a sequence $b$ of length $l + 1$, such that $b_1 = x$, $b_{l + 1} = y$, and for all $1\leq i\leq l$, $b_i$ has a smaller rank than $b_{i + 1}$ in at least one contest.

There are $q$ queries. In the $i$-th query, SolarPea is contestant $x$ and PolarSea is contestant $y$. Please find the minimum positive number $l$ such that SolarPea is $l$-stronger than PolarSea.

## �����ʽ
The first line contains two integers $n$ ($2\leq n\leq 10 ^ 5$) and $m$ ($1\leq m\leq 5$).

The $i$-th of the next $m$ lines contains $n$ intergers $a_{i, 1}, a_{i, 2}, \ldots, a_{i, n}$. It is guaranteed that $a_i$ is a permutaion of $1,2,\ldots,n$.

The next line contains an integer $q$ ($1\leq q\leq 10 ^ 5$).

Each of the next $q$ lines contains two integers $x$ and $y$ ($1 \le x,y \le n, x \neq y$), representing a query.

## �����ʽ
For each query, output a number $l$ representing the answer. If there is no legal $l$, output $-1$.

## ��Ŀ����
### ��Ŀ����

$n$ ��ѡ�ֲμ��� $m$ ������������ÿ�����������а񡣵� $k$ �����������а���һ�� $n$ ������ $a_k$����ʾѡ�� $a_{k, i}$ ������Ϊ $i$��

SolarPea �� PolarSea Ҳ��ѡ�֡�SolarPea ��Ҫ֤������ PolarSea ��ǿ��

����ѡ�� $x$��$l$ - ǿ�ڡ�ѡ�� $y$�����ҽ������ڳ���Ϊ $l + 1$ �����У����� $b_1 = x$��$b_{l + 1} = y$���Ҷ������� $1\leq i\leq l$������ $b_i$ ������һ������������С�� $b_{i + 1}$��

���� $q$ ��ѯ�ʡ��ڵ� $i$ ��ѯ���У�SolarPea ��ѡ�� $x$��PolarSea ��ѡ�� $y$�������С�������� $l$��ʹ�� $x$��$l$ - ǿ�ڡ�$y$��

$2\leq n\leq 10 ^ 5$��$1\leq q\leq 10 ^ 5$��$1\leq m\leq 5$��$1\leq x, y\leq n$��$x\neq y$��

### �����ʽ

��һ���������� $n, m$��

������ $m$ �У�ÿ�� $n$ ����������ʾ�� $i$ �����������а񡣱�֤ $a_i$ �� $1, 2, \ldots, n$ �����С�

������һ��һ������ $q$��

������ $q$ �У�ÿ���������� $x, y$ ��ʾһ��ѯ�ʡ�

### �����ʽ

����ÿ��ѯ�ʣ����һ��һ��������ʾ�𰸡��������������� $l$����� $-1$��



```input1
6 2
1 3 2 5 4 6
2 1 4 3 6 5
4
1 4
5 3
6 1
5 2

```

```output1
1
2
5
3

```

## ��ʾ
**Source**: The 2022 ICPC Asia Xi'an Regional Contest Problem D.

**Author**: csy2005.

