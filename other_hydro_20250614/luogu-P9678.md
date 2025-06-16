## ��Ŀ����
You are given an unrooted weighted tree $T$ with vertices $1, 2, \ldots, n$. Please answer some queries.

We define $\texttt{dist}(i,j)$ as the distance between vertex $i$ and vertex $j$ in $T$.

For each query, you are given two integers $l, r$. Please answer the value of 

$$\min_{l\le i< j\le r}(\texttt{dist}(i,j)).$$

## �����ʽ
The first line contains one integer $n~(1\leq n\le 2 \times 10^5)$, the number of vertices in the tree. 

Each of the next $n-1$ lines describes an edge of the tree. Edge $i$ is denoted by three integers $a_i, b_i, w_i$ $(1\le a_i, b_i\le n, 1\le w_i\le 10^9)$, the labels of vertices it connects and its weight. 

Then one line contains one integer $q~(1\leq q\le 10^6)$, the number of queries.

Each of the following $q$ lines contains two integers $l, r~(1\le l \le r\le n)$ describing a query.

It is guaranteed that the given edges form a tree.

## �����ʽ

For each query, output the answer in one line. If there is no $i,j$ such that $l\le i<j\le r$, the answer is $-1$.

## ��Ŀ����
����һ�� $n$ ����������� $\operatorname{dist}(i,j)$ Ϊ���� $i,j$ ֮��Ψһ��·���ĳ��ȡ�

��Ҫ�ش� $q$ ��ѯ�ʣ����� $l,r$���� $\min\limits_{l\leq i<j\leq r}(\operatorname{dist}(i,j))$��

```input1
5
1 2 5
1 3 3
1 4 4
3 5 2
5
1 1
1 4
2 4
3 4
2 5

```

```output1
-1
3
7
7
2

```

