## ��Ŀ����
Prof. Pang works for the City Brain program of Capital Grancel. The road network of Grancel can be represented by an undirected graph. Initially, the speed limit on each road is $1$m/s. Prof. Pang can increase the speed limit on a road by $1$m/s with the cost of $1$ dollar. Prof. Pang has $k$ dollars. He can spend any nonnegative integral amount of money on each road. If the speed limit on some road is $a$m/s, it takes $1/a$ seconds for anyone to go through the road in either direction.

After Prof. Pang spent his money, Prof. Du starts to travel from city $s_1$ to city $t_1$ and Prof. Wo starts to travel from city $s_2$ to city $t_2$. Help Prof. Pang to spend his money wisely to minimize the sum of minimum time of Prof. Du's travel and Prof. Wo's travel. It is guaranteed that $s_1$ and $t_1$ are connected by at least one path and that $s_2$ and $t_2$ are connected by at least one path.

## �����ʽ
The first line contains three integers $n$, $m$, $k$ ($1\le n \le 5000$, $0\le m \le 5000$, $0\le k\le 10^9$) separated by single spaces denoting the number of vertices, the number of edges in the graph and the number of dollars Prof. Pang has.

Each of the following $m$ lines contains two integers $a$, $b$ ($1\le a, b\le n, a\neq b$) separated by a single space denoting the two endpoints of one road. There can be multiple roads between the same pair of cities.

The following line contains four integers $s_1$, $t_1$, $s_2$, $t_2$ ($1\le s_1, t_1, s_2, t_2\le n$) separated by single spaces denoting the starting vertices and ending vertices of Prof. Du and Prof. Wo's travels.

## �����ʽ
Output one decimal in the only line -- the minimum sum of Prof. Du's travel time and Prof. Wo's travel time. The answer will be considered correct if its absolute or relative error does not exceed $10^{-9}$.

```input1
6 5 1
1 2
3 2
2 4
4 5
4 6
1 5 3 6
```

```output1
5.000000000000
```

```input2
1 0 100
1 1 1 1
```

```output2
0.000000000000
```

```input3
4 2 3
1 2
3 4
1 2 3 4
```

```output3
0.833333333333
```

