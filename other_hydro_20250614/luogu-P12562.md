## 题目描述
You are given two equal undirected trees $G$ and $H$ consisting of $n$ vertices. Trees are equal if, for all pairs of vertices $(u;v)$, the edge between $G_u$ and $G_v$ exists if and only if the edge between $H_u$ and $H_v$ exists.  

Some vertices can be connected to their version in another tree with an undirected edge. Especially, a leaf vertex $G_v$ can be connected to vertex $H_v$. Let us say that if leaf vertex $G_v$ is connected to $H_v$ directly, then vertex $v$ is **enabled**, and the vertex is **disabled** otherwise.

Initially, all leaf vertices are **disabled**. You are asked to handle the following queries:

- $1$ $v$ --- toggle the status of vertex $v$, if $v$ is **disabled** then change its status to **enabled** and vice versa otherwise;
- $2$ $u$ $v$ --- print the length of the shortest path from vertex $G_u$ to vertex $H_v$.

## 输入格式
The first line contains two integers $n$ and $q$ ($3 \le n \le 2 \cdot 10^5$; $1 \le q \le 2 \cdot 10^5$) --- number of vertices and queries, respectively.

Each of the following $n-1$ lines contains two integers $u$, $v$ $(1 \le u,v \le n)$ --- description of trees, edges $(G_u;G_v)$ and $(H_u;H_v)$.

Each of the following $q$ lines contains a description of queries. There are two possible query descriptions:

- $1$ $v$ $(1 \le v \le n)$ --- toggle the status of vertex $v$;
- $2$ $u$ $v$ $(1 \le u,v \le n)$ --- print the length of the shortest path from vertex $G_u$ to $H_v$.

## 输出格式
For each query of the second type, print a single integer in a single line --- the length of the shortest path between given vertices. If there is no such path, print $\texttt{-1}$.

```input1
7 11
1 2
2 3
1 4
2 5
4 6
4 7
1 6
1 3
2 1 6
2 1 2
1 7
2 5 4
2 6 3
1 6
1 3
1 5
2 6 3
```

```output1
2
3
5
4
6
```

```input2
3 2
1 2
1 3
1 3
2 1 2
```

```output2
3
```

## 提示
Let $k$ be the number of queries of the second type.

- ($3$ points): $n \le 16$, $q \le 16$;
- ($3$ points): $n \le 16$, $q \le 2 \cdot 10^5$;
- ($2$ points): $n \le 2000$, $q \le 2 \cdot 10^5,k \le 5$;
- ($8$ points): $n \le 2000$, $q \le 2000$;
- ($9$ points): $n \le 2 \cdot 10^5$, $q \le 2 \cdot 10^5, k \le 5$;
- ($30$ points): $n \le 2 \cdot 10^5$, $q \le 2 \cdot 10^5$, there is no query of first type after query of second type;
- ($45$ points): no additional restrictions.

