## Description

<div><p>You are given an undirected graph consisting of $n$ vertices. A number is written on each vertex; the number on vertex $i$ is $a_i$. Initially there are no edges in the graph.</p><p>You may add some edges to this graph, but you have to pay for them. The cost of adding an edge between vertices $x$ and $y$ is $a_x + a_y$ coins. There are also $m$ special offers, each of them is denoted by three numbers $x$, $y$ and $w$, and means that you can add an edge connecting vertices $x$ and $y$ and pay $w$ coins for it. You don't have to use special offers: if there is a pair of vertices $x$ and $y$ that has a special offer associated with it, you still may connect these two vertices paying $a_x + a_y$ coins for it.</p><p>What is the minimum number of coins you have to spend to make the graph connected? Recall that a graph is connected if it's possible to get from any vertex to any other vertex using only the edges belonging to this graph.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$, $0 \le m \le 2 \cdot 10^5$) ！ the number of vertices in the graph and the number of special offers, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^{12}$) ！ the numbers written on the vertices.</p><p>Then $m$ lines follow, each containing three integers $x$, $y$ and $w$ ($1 \le x, y \le n$, $1 \le w \le 10^{12}$, $x \ne y$) denoting a special offer: you may add an edge connecting vertex $x$ and vertex $y$, and this edge will cost $w$ coins.</p></div><div class="output-specification"><p>Print one integer ！ the minimum number of coins you have to pay to make the graph connected.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 2 \cdot 10^5$, $0 \le m \le 2 \cdot 10^5$) ！ the number of vertices in the graph and the number of special offers, respectively.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^{12}$) ！ the numbers written on the vertices.</p><p>Then $m$ lines follow, each containing three integers $x$, $y$ and $w$ ($1 \le x, y \le n$, $1 \le w \le 10^{12}$, $x \ne y$) denoting a special offer: you may add an edge connecting vertex $x$ and vertex $y$, and this edge will cost $w$ coins.</p>

## Output

<p>Print one integer ！ the minimum number of coins you have to pay to make the graph connected.</p>

## Samples

```input1
3 2
1 3 3
2 3 5
2 1 1
```

```output1
5
```






```input2
4 0
1 3 3 7
```

```output2
16
```






```input3
5 4
1 2 3 4 5
1 2 8
1 3 10
1 4 7
1 5 15
```

```output3
18
```




## Note

<p>In the first example it is possible to connect $1$ to $2$ using special offer $2$, and then $1$ to $3$ without using any offers.</p><p>In next two examples the optimal answer may be achieved without using special offers.</p>
