## Description

<div><p>You are given a connected undirected graph, the vertices of which are numbered with integers from $1$ to $n$. Your task is to minimize the number of pairs of vertices $1 \leq u &lt; v \leq n$ between which there exists a path in this graph. To achieve this, you can remove exactly one edge from the graph.</p><p>Find the smallest number of pairs of vertices!</p></div><div class="input-specification"><p>Each test consists of several sets of input data. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of sets of input data. Then follows their description.</p><p>The first line of each set of input data contains two integers $n$ and $m$ ($2 \leq n \leq 10^5$, $n - 1 \leq m \leq \min(10^5, \frac{n \cdot (n - 1)}{2})$)&nbsp;！ the number of vertices in the graph and the number of edges.</p><p>Each of the next $m$ lines contains two integers $u$ and $v$ ($1 \leq u, v \leq n, u \neq v$), indicating that there is an undirected edge in the graph between vertices $u$ and $v$.</p><p>It is guaranteed that the given graph is connected and without multiple edges.</p><p>It is guaranteed that the sum of $n$ and the sum of $m$ over all sets of input data does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each set of input data, output the smallest number of pairs of reachable vertices, if exactly one edge can be removed.</p></div>

## Input

<p>Each test consists of several sets of input data. The first line contains a single integer $t$ ($1 \leq t \leq 10^4$)&nbsp;！ the number of sets of input data. Then follows their description.</p><p>The first line of each set of input data contains two integers $n$ and $m$ ($2 \leq n \leq 10^5$, $n - 1 \leq m \leq \min(10^5, \frac{n \cdot (n - 1)}{2})$)&nbsp;！ the number of vertices in the graph and the number of edges.</p><p>Each of the next $m$ lines contains two integers $u$ and $v$ ($1 \leq u, v \leq n, u \neq v$), indicating that there is an undirected edge in the graph between vertices $u$ and $v$.</p><p>It is guaranteed that the given graph is connected and without multiple edges.</p><p>It is guaranteed that the sum of $n$ and the sum of $m$ over all sets of input data does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each set of input data, output the smallest number of pairs of reachable vertices, if exactly one edge can be removed.</p>





```input1|2,3,8,9,10,11,12,13,22,23,24,25,26,27
6
2 1
1 2
3 3
1 2
2 3
1 3
5 5
1 2
1 3
3 4
4 5
5 3
6 7
1 2
1 3
2 3
3 4
4 5
4 6
5 6
5 5
1 2
1 3
2 3
2 4
3 5
10 12
1 2
1 3
2 3
2 4
4 5
5 6
6 7
7 4
3 8
8 9
9 10
10 8
```




```output1
0
3
4
6
6
21
```



## Note

<p>In the first set of input data, we will remove the single edge $(1, 2)$ and the only pair of vertices $(1, 2)$ will become unreachable from each other.</p><p>In the second set of input data, no matter which edge we remove, all vertices will be reachable from each other.</p><p>In the fourth set of input data, the graph looks like this initially.</p><center> <img class="tex-graphics" src="./34757/file/cKUx3zeV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>We will remove the edge $(3, 4)$ and then the only reachable pairs of vertices will be $(1, 2)$, $(1, 3)$, $(2, 3)$, $(4, 5)$, $(4, 6)$, $(5, 6)$.</p><center> <img class="tex-graphics" src="./34757/file/K6FBzt1p.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the sixth set of input data, the graph looks like this initially.</p><center> <img class="tex-graphics" src="./34757/file/drkklq9k.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>After removing the edge $(2, 4)$, the graph will look like this. Thus, there will be $21$ pairs of reachable vertices.</p><center> <img class="tex-graphics" src="./34757/file/S6cacX9V.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
