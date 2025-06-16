## ��Ŀ����
We are given a tree with N nodes denoted with different positive integers from 1 to N.
Additionally, you are given M node pairs from the tree in the form of ($a_1$
, $b_1$
), ($a_2$
, $b_2$
), ��, ($a_M$
,
$b_M$
).

We need to direct each edge of the tree so that for each given node pair ($a_i$
, $b_i$
) there is a
path from $a_i$
to $b_i$ or from $b_i$
to $a_i$
. How many different ways are there to achieve this?
Since the solution can be quite large, determine it modulo $10^{9}+7$.


## �����ʽ
The first line of input contains the positive integers N and M (1 �� N, M �� $3*10^5$), the number of
nodes in the tree and the number of given node pairs, respectively.

Each of the following N - 1 lines contains two positive integers, the labels of the nodes
connected with an edge.

The $i_{th}$ of the following M lines contains two different positive integers $a_{i}$ and $b_{i}$
, the labels of
the nodes from the $i_{th}$ node pair. All node pairs will be mutually different.


## �����ʽ
You must output a single line containing the total number of different ways to direct the
edges of the tree that meet the requirement from the task, modulo $10^{9}+7$.


## ��Ŀ����
����һ�Ŵ�1��n��ŵ�n��������

ͬʱ����m��Լ��������$(a_i,b_i)$

��ÿһ���߶���ʹ�ö���ÿһ��Լ���Դ���һ����$a_i$��$b_i$���$b_i$��$a_i$��·����

����еķ��������𰸶�$10^9 + 7$ȡģ

$1 \le n,m \le 3 \times 10^5$

```
����һ�Ŵ�1��n��ŵ�n��������

ͬʱ����m��Լ��������$(a_i,b_i)$

��ÿһ���߶���ʹ��ÿһ��Լ���Դ���һ����$a_i$��$b_i$���$b_i$��$a_i$��·����

����еķ��������𰸶�$10^9 + 7$ȡģ

$1 \le n,m \le 3 \times 10^5$
```

```input1
4 1
1 2
2 3
3 4
2 4
```

```output1
4
```

```input2
7 2
1 2
1 3
4 2
2 5
6 5
5 7
1 7
2 6

```

```output2
8
```

```input3
4 3
1 2
1 3
1 4
2 3
2 4
3 4

```

```output3
0
```

## ��ʾ
In test cases worth 20% of total points, the given tree will be a chain. In other words, node i
will be connected with an edge to node i + 1 for all i < N.

In additional test cases worth 40% of total points, it will hold N, M �� $5*10^3$.

A tree is a graph that consists of N nodes and N - 1 edges such that there exists a path from each
node to each other node.

