## Description

<div><p>You are given an undirected graph consisting of $n$ vertices and $m$ edges.</p><p>Recall that a cycle is a path that starts and ends in the same vertex. A cycle in a graph is called simple if it contains each vertex (except the starting and ending one) no more than once (the starting and the ending one is contained always <span class="tex-font-style-bf">twice</span>). Note that loops are considered to be simple cycles.</p><p>In one move you can choose <span class="tex-font-style-bf">any</span> simple cycle in this graph and erase the edges corresponding to this cycle (corresponding vertices remain in the graph). It is <span class="tex-font-style-bf">allowed</span> to erase the loop or two copies of the same edge (take a look at examples).</p><p>Your problem is to apply some sequence of moves to obtain the graph without edges. <span class="tex-font-style-bf">It is not necessary to minimize the number of cycles</span>. If it is impossible, print "<span class="tex-font-style-tt">NO</span>".</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) ！ the number of vertices and the number of edges in the graph.</p><p>The next $m$ lines contain edges of the graph. The $i$-th line contains the $i$-th edge $x_i, y_i$ ($1 \le x_i, y_i \le n$), where $x_i$ and $y_i$ are vertices connected by the $i$-th edge. The graph <span class="tex-font-style-bf">can contain loops or multiple edges</span>.</p></div><div class="output-specification"><p>If it is impossible to decompose the given graph into simple cycles, print "<span class="tex-font-style-tt">NO</span>" in the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line. In the second line print $k$ ！ the number of simple cycles in the graph decomposition.</p><p>In the next $k$ lines print cycles themselves. The $j$-th line should contain the $j$-th cycle. First, print $c_j$ ！ the number of vertices in the $j$-th cycle. Then print the cycle as a sequence of vertices. All neighbouring (adjacent) vertices in the printed path should be connected by an edge that isn't contained in other cycles.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $m$ ($1 \le n, m \le 2 \cdot 10^5$) ！ the number of vertices and the number of edges in the graph.</p><p>The next $m$ lines contain edges of the graph. The $i$-th line contains the $i$-th edge $x_i, y_i$ ($1 \le x_i, y_i \le n$), where $x_i$ and $y_i$ are vertices connected by the $i$-th edge. The graph <span class="tex-font-style-bf">can contain loops or multiple edges</span>.</p>

## Output

<p>If it is impossible to decompose the given graph into simple cycles, print "<span class="tex-font-style-tt">NO</span>" in the first line.</p><p>Otherwise print "<span class="tex-font-style-tt">YES</span>" in the first line. In the second line print $k$ ！ the number of simple cycles in the graph decomposition.</p><p>In the next $k$ lines print cycles themselves. The $j$-th line should contain the $j$-th cycle. First, print $c_j$ ！ the number of vertices in the $j$-th cycle. Then print the cycle as a sequence of vertices. All neighbouring (adjacent) vertices in the printed path should be connected by an edge that isn't contained in other cycles.</p>

## Samples

```input1
6 9
1 2
2 3
1 3
2 4
2 5
4 5
3 5
3 6
5 6
```

```output1
YES
3
4 2 5 4 2 
4 3 6 5 3 
4 1 3 2 1
```






```input2
4 7
1 1
1 2
2 3
3 4
4 1
1 3
1 3
```

```output2
YES
3
2 1 1 
5 1 4 3 2 1 
3 1 3 1
```






```input3
4 8
1 1
1 2
2 3
3 4
4 1
2 4
1 3
1 3
```

```output3
NO
```




## Note

<p>The picture corresponding to the first example: <img class="tex-graphics" src="./30201/file/vBZEkYuI.png" style="max-width: 100.0%;max-height: 100.0%;"></p>
