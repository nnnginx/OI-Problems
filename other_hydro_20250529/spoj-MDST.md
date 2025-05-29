<p>Solve the minimum diameter spanning tree problem for the simple graphs.
</p><p>For a given list of adjacent vertices of a graph G find the minimum diameter spanning tree T and write down the diameter of this tree diam(T). 
</p><p>Each graph has only one connected component, so there is at least one spanning tree, which connects all the vertices.

</p><h3>Input</h3>
<p>t [the number of test graphs]<br>
Graph:<br>
<i>n</i> [1 &lt;= <i>n</i> &lt;= 1000 the number of graph vertices]<br>
<i>i m v<sub>1</sub> v<sub>2</sub> ... v<sub>m</sub></i> [the list of <i>m</i> adjacent vertices to vertex <i>i</i>]

</p><h3>Output</h3>
<p>For each test case output:<br>
<i>d</i> [diameter of the minimum diameter spanning tree]

</p><h3>Example</h3>

<pre><b>Input:</b>
6

10
1 3 2 3 4
2 3 1 5 7
3 3 1 5 6
4 3 1 6 8
5 3 2 3 9
6 3 3 4 10
7 1 2
8 1 4
9 1 5
10 1 6

10
1 4 4 5 7 9
2 1 8
3 4 4 7 8 10
4 3 1 3 9
5 2 1 9
6 2 8 9
7 4 1 3 8 9
8 5 2 3 6 7 9
9 7 1 4 5 6 7 8 10
10 2 3 9

1
1 0

2
1 1 2
2 1 1

3
1 1 2
2 2 1 3
3 1 2

5
1 2 2 4
2 3 1 3 4
3 1 2
4 3 2 5 1
5 1 4

<b>Output:</b>
5
3
0
1
2
3

</pre>