## Description

<div><p>You are given a connected undirected weighted graph consisting of $n$ vertices and $m$ edges.</p><p>You need to print the $k$-th smallest shortest path in this graph (paths from the vertex to itself are not counted, paths from $i$ to $j$ and from $j$ to $i$ are counted as one).</p><p>More formally, if $d$ is the matrix of shortest paths, where $d_{i, j}$ is the length of the shortest path between vertices $i$ and $j$ ($1 \le i &lt; j \le n$), then you need to print the $k$-th element in the sorted array consisting of all $d_{i, j}$, where $1 \le i &lt; j \le n$.</p></div><div class="input-specification"><p>The first line of the input contains three integers $n, m$ and $k$ ($2 \le n \le 2 \cdot 10^5$, $n - 1 \le m \le \min\Big(\frac{n(n-1)}{2}, 2 \cdot 10^5\Big)$, $1 \le k \le \min\Big(\frac{n(n-1)}{2}, 400\Big)$&nbsp;�� the number of vertices in the graph, the number of edges in the graph and the value of $k$, correspondingly.</p><p>Then $m$ lines follow, each containing three integers $x$, $y$ and $w$ ($1 \le x, y \le n$, $1 \le w \le 10^9$, $x \ne y$) denoting an edge between vertices $x$ and $y$ of weight $w$.</p><p>It is guaranteed that the given graph is <span class="tex-font-style-bf">connected</span> (there is a path between any pair of vertices), there are no self-loops (edges connecting the vertex with itself) and multiple edges (for each pair of vertices $x$ and $y$, there is at most one edge between this pair of vertices in the graph).</p></div><div class="output-specification"><p>Print one integer&nbsp;�� the length of the $k$-th smallest shortest path in the given graph (paths from the vertex to itself are not counted, paths from $i$ to $j$ and from $j$ to $i$ are counted as one).</p></div>

## Input

<p>The first line of the input contains three integers $n, m$ and $k$ ($2 \le n \le 2 \cdot 10^5$, $n - 1 \le m \le \min\Big(\frac{n(n-1)}{2}, 2 \cdot 10^5\Big)$, $1 \le k \le \min\Big(\frac{n(n-1)}{2}, 400\Big)$&nbsp;�� the number of vertices in the graph, the number of edges in the graph and the value of $k$, correspondingly.</p><p>Then $m$ lines follow, each containing three integers $x$, $y$ and $w$ ($1 \le x, y \le n$, $1 \le w \le 10^9$, $x \ne y$) denoting an edge between vertices $x$ and $y$ of weight $w$.</p><p>It is guaranteed that the given graph is <span class="tex-font-style-bf">connected</span> (there is a path between any pair of vertices), there are no self-loops (edges connecting the vertex with itself) and multiple edges (for each pair of vertices $x$ and $y$, there is at most one edge between this pair of vertices in the graph).</p>

## Output

<p>Print one integer&nbsp;�� the length of the $k$-th smallest shortest path in the given graph (paths from the vertex to itself are not counted, paths from $i$ to $j$ and from $j$ to $i$ are counted as one).</p>

## Samples

```input1
6 10 5
2 5 1
5 3 9
6 2 2
1 3 1
5 1 8
6 5 10
1 6 5
6 4 6
3 6 2
3 4 5
```

```output1
3
```






```input2
7 15 18
2 6 3
5 7 4
6 5 4
3 6 9
6 7 7
1 6 4
7 1 6
7 2 1
4 3 2
3 2 8
5 3 6
2 5 5
3 7 9
4 1 8
2 1 1
```

```output2
9
```



