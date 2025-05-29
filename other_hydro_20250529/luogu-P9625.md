## ��Ŀ����
Given an undirected connected graph with $n$ vertices and $m$ edges, your task is to find a spanning tree of the graph such that for every vertex in the spanning tree its degree is not larger than $\frac{n}{2}$.

Recall that the degree of a vertex is the number of edges it is connected to.

## �����ʽ
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $m$ ($2 \le n \le 10^5$, $n-1 \le m \le 2 \times 10^5$) indicating the number of vertices and edges in the graph.

For the following $m$ lines, the $i$-th line contains two integers $u_i$ and $v_i$ ($1 \le u_i, v_i \le n$) indicating that there is an edge connecting vertex $u_i$ and $v_i$. Please note that there might be self loops or multiple edges.

It's guaranteed that the given graph is connected. It's also guaranteed that the sum of $n$ of all test cases will not exceed $5 \times 10^5$, also the sum of $m$ of all test cases will not exceed $10^6$.


## �����ʽ
For each test case, if such spanning tree exists first output ``Yes`` in one line, then for the following $(n-1)$ lines print two integers $p_i$ and $q_i$ on the $i$-th line separated by one space, indicating that there is an edge connecting vertex $p_i$ and $q_i$ in the spanning tree. If no valid spanning tree exists just output ``No`` in one line.


## ��Ŀ����
### ��Ŀ����

����һ�� $n$ ���� $m$ ���ߵ�����ͼ����һ������������ÿ����Ķ����������� $\frac{n}{2}$��

### �����ʽ

�������ݣ���һ�У�һ������ $t$ ��������������

����ÿ�����ݣ�

- ��һ���������� $n$, $m$����������͵�����
- ������ $m$ �У����� $u_i,v_i$ ����һ���ߣ��������رߺ��Ի�����

### �����ʽ

����ÿ�����ݣ�

��һ����� `Yes` �� `No` �����Ƿ���С�

�����У������� $n - 1$ �����ÿ���������ıߣ�˳�����⡣

### ���ݷ�Χ

$2 \leq n \leq 10^5$��$n - 1\leq m \leq 2\times10^5$��$\sum n\leq5\times10^5$��$\sum m\leq10^6$��

��֤ͼ��ͨ��

```input1
2
6 9
1 2
1 3
1 4
2 3
2 4
3 4
4 5
4 6
4 6
3 4
1 3
2 3
3 3
1 2

```

```output1
Yes
1 2
1 3
1 4
4 5
4 6
No

```

## ��ʾ
### Note

For the first sample test case, the maximum degree among all vertices in the spanning tree is 3 (both vertex 1 and vertex 4 has a degree of 3). As $3 \le \frac{6}{2}$ this is a valid answer.

For the second sample test case, it's obvious that any spanning tree will have a vertex with degree of 2, as $2 > \frac{3}{2}$ no valid answer exists.


