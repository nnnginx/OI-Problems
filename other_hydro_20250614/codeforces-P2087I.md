## Description

<div><p>You are given a directed acyclic graph with $n$ vertices and $m$ edges. The graph contains no cycles or multiple edges.</p><p>You need to partition all the edges of this graph into Hamiltonian cycles (cycles that visit each of the $n$ vertices of the graph exactly once) such that each edge belongs to exactly one cycle. It is obvious that this is impossible for the original graph, so before partitioning, you must add the <span class="tex-font-style-bf">minimum</span> number of edges to the graph so that such a partition exists.</p><p>After adding edges, the graph may contain cycles and/or multiple edges, but it should still not have any self-loops.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($2 \le n \le 100$; $1 \le m \le \frac{n(n-1)}{2}$).</p><p>The next $m$ lines contain two integers $x_i$ and $y_i$ in the $i$-th line ($1 \le x_i, y_i \le n$; $x_i \ne y_i$), representing a directed edge from vertex $x_i$ to vertex $y_i$.</p><p>Additional constraints on the input:</p><ul> <li> the given graph has no cycles or multiple edges. </li></ul></div><div class="output-specification"><p>In the first line, output a single integer $k$ ($1 \le k \le n \cdot m$) ！ the number of edges you add.</p><p>Then output $k$ lines, in the $i$-th of which there should be two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$; $x_i \ne y_i$), denoting the start and end of the next edge.</p><p>Then in a single line, output a single integer $c$ ($1 \le c \le m$) ！ the number of Hamiltonian cycles into which you partition all the edges of the graph.</p><p>In the last line, output $m+k$ integers $a_1, a_2, \dots, a_{m+k}$ ($1 \le a_i \le c$), where $a_i$ is the Hamiltonian cycle to which you assign the $i$-th edge (the edges of the original graph are numbered from $1$ to $m$, and the new ones are from $m+1$ to $m+k$).</p><p>If there are multiple answers that minimize the number of added edges, output any of them.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($2 \le n \le 100$; $1 \le m \le \frac{n(n-1)}{2}$).</p><p>The next $m$ lines contain two integers $x_i$ and $y_i$ in the $i$-th line ($1 \le x_i, y_i \le n$; $x_i \ne y_i$), representing a directed edge from vertex $x_i$ to vertex $y_i$.</p><p>Additional constraints on the input:</p><ul> <li> the given graph has no cycles or multiple edges. </li></ul>

## Output

<p>In the first line, output a single integer $k$ ($1 \le k \le n \cdot m$) ！ the number of edges you add.</p><p>Then output $k$ lines, in the $i$-th of which there should be two integers $x_i$ and $y_i$ ($1 \le x_i, y_i \le n$; $x_i \ne y_i$), denoting the start and end of the next edge.</p><p>Then in a single line, output a single integer $c$ ($1 \le c \le m$) ！ the number of Hamiltonian cycles into which you partition all the edges of the graph.</p><p>In the last line, output $m+k$ integers $a_1, a_2, \dots, a_{m+k}$ ($1 \le a_i \le c$), where $a_i$ is the Hamiltonian cycle to which you assign the $i$-th edge (the edges of the original graph are numbered from $1$ to $m$, and the new ones are from $m+1$ to $m+k$).</p><p>If there are multiple answers that minimize the number of added edges, output any of them.</p>





```input1|
3 2
1 2
2 3
```




```input2|
5 4
1 2
3 2
3 4
5 4
```




```input3|
4 6
1 2
2 4
4 3
1 3
2 3
1 4
```




```output1
1
3 1
1
1 1 1
```




```output2
6
2 3
4 5
5 1
1 5
2 1
4 3
2
1 2 1 2 1 1 1 2 2 2
```




```output3
6
3 1
4 2
3 1
3 2
2 4
4 1
3
1 1 1 3 2 2 1 2 2 3 3 3
```


