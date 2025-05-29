## Description

<div><p>A connected component of an undirected graph is defined as a set of vertices $S$ of this graph such that:</p><ul> <li> for every pair of vertices $(u, v)$ in $S$, there exists a path between vertices $u$ and $v$; </li><li> there is no vertex outside $S$ that has a path to a vertex within $S$. </li></ul><p>For example, the graph in the picture below has three components: $\{1, 3, 7, 8\}$, $\{2\}$, $\{4, 5, 6\}$.</p><center> <img class="tex-graphics" src="./35708/file/DSKP9rI2.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>We say that graph $A$ <span class="tex-font-style-it">includes</span> graph $B$ if every component of graph $B$ is a subset of some component of graph $A$.</p><p>You are given two graphs, $A$ and $B$, both consisting of $n$ vertices numbered from $1$ to $n$. Initially, there are no edges in the graphs. You must process queries of two types:</p><ul> <li> add an edge to one of the graphs; </li><li> remove an edge from one of the graphs. </li></ul><p>After each query, you have to calculate the minimum number of edges that have to be added to $A$ so that $A$ includes $B$, and print it. Note that you don't actually add these edges, you just calculate their number.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($2 \le n \le 4 \cdot 10^5$; $1 \le q \le 4 \cdot 10^5$) ！ the number of vertices and queries, respectively.</p><p>Next, there are $q$ lines, where the $i$-th line describes the $i$-th query. The description of the query begins with the character $c_i$ (either <span class="tex-font-style-tt">A</span> or <span class="tex-font-style-tt">B</span>) ！ the graph to which the query should be applied. Then, two integers $x_i$ and $y_i$ follow ($1 \le x_i, y_i \le n$; $x_i \ne y_i$). If there is an edge $(x_i, y_i)$ in the corresponding graph, it should be removed; otherwise, it should be added to that graph.</p></div><div class="output-specification"><p>For each query, print one integer ！ the minimum number of edges that you have to add to the graph $A$ so that it includes $B$.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($2 \le n \le 4 \cdot 10^5$; $1 \le q \le 4 \cdot 10^5$) ！ the number of vertices and queries, respectively.</p><p>Next, there are $q$ lines, where the $i$-th line describes the $i$-th query. The description of the query begins with the character $c_i$ (either <span class="tex-font-style-tt">A</span> or <span class="tex-font-style-tt">B</span>) ！ the graph to which the query should be applied. Then, two integers $x_i$ and $y_i$ follow ($1 \le x_i, y_i \le n$; $x_i \ne y_i$). If there is an edge $(x_i, y_i)$ in the corresponding graph, it should be removed; otherwise, it should be added to that graph.</p>

## Output

<p>For each query, print one integer ！ the minimum number of edges that you have to add to the graph $A$ so that it includes $B$.</p>





```input1|
6 9
A 2 3
B 1 3
A 2 1
A 3 2
B 5 6
A 6 5
A 3 4
A 4 2
A 4 3
```




```output1
0
1
0
1
2
1
1
0
1
```


