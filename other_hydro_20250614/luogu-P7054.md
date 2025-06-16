## ��Ŀ����


The sequence $a_{1}, a_{2},$ . . . , $a_{n}$ is called a permutation, if it contains every integer from $1$ to $n$ .

The permutation of vertices $a_{1}, a_{2},$ . . . , $a_{n}$ is a topological sort of a directed graph, if for every directed edge from $u$ to $v$ , vertex $u$ comes before $v$ in this permutation.

The permutation $a_{1}, a_{2},$ . . . , $a_{n}$ is lexicographically smaller than the permutation $b_{1}, b_{2},$ . . . , $b_{n},$ if there exists $m$ such that $a_{i} = b_{i}$ for every $1 \le i < m$ and $a_{m} < b_{m}.$

Given a directed acyclic graph, add at most $k$ directed edges to it in such a way, that the resulting graph still has no cycles and the lexicographically minimal topological sort of the graph is maximum possible.



## �����ʽ


The first line of the input file contains three integers $n , m$ and $k$ -- the number of vertices and directed edges in the original graph, and the number of directed edges, that you are allowed to add $(1 \le n \le 100 000$ ; $0 \le m , k \le 100 000)$ .

Each of the following $m$ lines contains two integers $u_{i}, v_{i},$ describing directed edge from $u_{i}$ to $v_{i} (1 \le u_{i}, v_{i} \le n)$ .

The graph has no cycles.



## �����ʽ


The first line of the output file should contain $n$ integers -- the lexicographically minimal topological sort of the modified graph. The second line should contain a single integer $x (0 \le x \le k)$ -- the number of directed edges to add. The following $x$ lines of the output should contain description of added directed edges in the same format as in the input file.



## ��Ŀ����
����һ�� $n$ �� $m$ ���ߵ������޻�ͼ�������������� $k$ ������ߣ�ʹ������Ȼ��һ�������޻�ͼ��ʹ���ֵ�����С����������ֵ�������

�������������Լ�������

$n,m,k\le 10^5$

```input1
5 3 2
1 4
4 2
1 3

```

```output1
5 1 4 2 3
2
4 3
5 1

```

```input2
2 2 20
1 2
1 2

```

```output2
1 2
1
1 2

```

## ��ʾ
Time limit: 2 s, Memory limit: 256 MB. 



