## ��Ŀ����
You are given a tree $T$ with $n$ nodes. The tree is rooted at $1$. Define $\mathrm{subtree}(u)$ as the set of nodes in the subtree of $u$.

Call a subset of nodes $S$ good if and only if $S$ satisfies at least one of the following contidions:

- For all $u, v\in S$ where $u\neq v$, either $u\in \mathrm{subtree}(v)$ or $v\in \mathrm{subtree}(u)$.
- For all $u, v\in S$ where $u\neq v$, both $u\notin \mathrm{subtree}(v)$ and $v\notin \mathrm{subtree}(u)$.

You need to partition all nodes of $T$ into several good subsets. Calculate the minimum number of subsets.


## �����ʽ
The first line contains a single integer $Q$ ($1\leq Q\leq 10 ^ 5$), denoting the number of test cases.

For each test case, the first line contains an integer $n$ ($1\leq n\leq 10 ^ 6$). The next line contains $n - 1$ integers $p_2, p_3, \ldots, p_n$ ($1\leq p_i < i$), indicating that there is an edge between $p_i$ and $i$ for each $i=2,3,\ldots,n$.

It is guaranteed that the sum of $n$ over all test cases is no more than $10 ^ 6$.

## �����ʽ
For each test case, output a single integer representing the answer.

## ��Ŀ����
### ��Ŀ����

������СΪ $n$ ���и��� $T$�����ڵ�Ϊ $1$������ $\mathrm{subtree}(u)$ ��ʾ��� $u$ ��������

�Ƽ��� $S$ �Ǻõģ����ҽ��� $S$ ����������������֮һ��

- ���� $u, v\in S$ �� $u\neq v$��$u\in \mathrm{subtree}(v)$ �� $v\in \mathrm{subtree}(u)$��
- ���� $u, v\in S$ �� $u\neq v$��$u\notin \mathrm{subtree}(v)$ �� $v\notin \mathrm{subtree}(u)$��

�� $T$ ����Ϊ���ɺõļ��ϣ��󼯺���������Сֵ��

���� $Q$ �����ݡ�

$1\leq Q\leq 10 ^ 5$��$1\leq n, \sum n\leq 10 ^ 6$��ÿ����ĸ��ױ�� $1\leq p_i < i$��

### �����ʽ

��һ��һ������ $Q$��

����ÿ��������ݣ���һ��һ������ $n$���ڶ��� $n - 1$ ���ɿո���������� $p_2, p_3, \cdots, p_n$����ʾÿ����ĸ��ױ�š�

### �����ʽ

����ÿ��������ݣ����һ��һ��������ʾ�𰸡�

```input1
2
7
1 1 2 2 2 3
5
1 2 3 4

```

```output1
3
1

```

## ��ʾ
**Source**: The 2022 ICPC Asia Xi'an Regional Contest Problem L.

**Author**: Alex_Wei.

