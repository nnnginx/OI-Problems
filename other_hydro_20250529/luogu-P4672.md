## ��Ŀ����
Let $T$ be a rooted tree (a connected undirected acylic graph), and let $S$ be a perfect copy of $T$. Construct a new graph by taking the union of $T$ and $S$, and merging the corresponding leaf nodes (but never the root). We call such a graph a tree-mirrored graph.

## �����ʽ
The first line of input contains two integers $N$ and $M$, the number of vertices and edges of a graph $G$. The vertices in $G$ are labeled from $1$ to $N$. The following $M$ lines describe the edges. Each such line contains two integers $x$ and $y(x��y;1 \le x,y \le N)$, describing one edge. There will be at most one edge between any pair of vertices.

## �����ʽ
The first and only line of output should contain the string ``YES`` if the graph $G$ is a tree-mirrored graph, and ``NO`` otherwise.

## ��Ŀ����
### ��Ŀ����

����һ���� $T$��������һ���� $T$ ͬ������ $S$������һ���µ�ͼ $T'$����ͼ $T'$ ͨ���ϲ� $T$ �� $S$ ����Ӧ�ķǸ�Ҷ�ڵ�õ������ǳ�������ͼΪ��֮����ͼ��

����һ��ͼ $G$������Ҫ�ж� $G$ �Ƿ�����֮����ͼ��

### ���������ʽ

#### �����ʽ��

����ĵ�һ�а����������� $N$ �� $M$����ʾͼ $G$ �Ķ���ͱ�����

�������� $M$ �У�ÿһ�а������������� $x$ �� $y$��$x \neq y$ �� $1 \leq x,y \leq n$����ʾ���� $x$ �� $y$ ֮����һ���ߡ���֤û���رߡ�

#### �����ʽ��

���ֻ��һ�У��ж�ͼ $G$ �Ƿ���һ����֮����ͼ������� `yes`��������� `no`��

Translated by @��Ѱ 

```input1
7 7
1 2
2 3
3 4
4 5
5 6
6 7
7 1
```

```output1
NO
```

```input2
6 6
1 2
2 3
2 4
3 5
4 5
5 6
```

```output2
YES
```

```input3
22 28
13 8
8 1
1 22
1 12
1 14
13 18
13 4
4 20
20 7
13 15
15 3
15 9
9 16
9 19
22 5
12 5
14 5
5 11
11 6
18 6
7 10
10 17
17 6
3 21
21 6
16 2
19 2
2 21
```

```output3
YES
```

## ��ʾ
���� $30\%$ �����ݣ�$3 \le N,M \le 300$��

���� $60\%$ �����ݣ�$3 \le N,M \le 3500$��

�����������ݣ�$3 \le N,M \le 10^5$��

