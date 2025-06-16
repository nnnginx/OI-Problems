## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>Kostyanych has chosen a complete undirected graph$^{\dagger}$ with $n$ vertices, and then removed exactly $(n - 2)$ edges from it. You can ask queries of the following type:</p><ul> <li> "<span class="tex-font-style-tt">?</span> $d$" ！ Kostyanych tells you the number of vertex $v$ with a degree <span class="tex-font-style-bf">at least</span> $d$. Among all possible such vertices, he selects the vertex <span class="tex-font-style-bf">with the minimum degree</span>, and if there are several such vertices, he selects the one with the minimum number. He also tells you the number of another vertex in the graph, with which $v$ is not connected by an edge (if none is found, then $0$ is reported). Among all possible such vertices, he selects the one with the minimum number. Then he removes the vertex $v$ and all edges coming out of it. If the required vertex $v$ is not found, then "$0\ 0$" is reported. </li></ul><p>Find a Hamiltonian path$^{\ddagger}$ in the <span class="tex-font-style-bf">original</span> graph in at most $n$ queries. It can be proven that under these constraints, a Hamiltonian path always exists.</p><p>$^{\dagger}$A complete undirected graph is a graph in which there is exactly one undirected edge between any pair of distinct vertices. Thus, a complete undirected graph with $n$ vertices contains $\frac{n(n-1)}{2}$ edges.</p><p>$^{\ddagger}$A Hamiltonian path in a graph is a path that passes through each vertex exactly once.</p></div><div class="input-specification"><p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single integer $n$ ($2 \le n \le 10^5$) ！ the number of vertices in the graph.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div><h2>Interaction</h2><p>Interaction for each test case begins with reading the integer $n$.</p><p>Then you can make no more than $n$ queries.</p><p>To make a query, output a line in the format "<span class="tex-font-style-tt">?</span> $d$" (without quotes) ($0 \le d \le n - 1$). After each query, read two integers&nbsp;！ the answer to your query.</p><p>When you are ready to report the answer, output a line in the format "<span class="tex-font-style-tt">!</span> $v_1\ v_2 \ldots v_n$" (without quotes)&nbsp;！ the vertices in the order of their occurrence in the Hamiltonian path. Outputting the answer does not count as one of the $n$ queries. After solving one test case, the program should immediately move on to the next one. After solving all test cases, the program should be terminated immediately.</p><p>If your program makes more than $n$ queries for one test case or makes an incorrect query, then the <span class="tex-font-style-bf">response to the query will be</span> $-1$, and after receiving such a response, your program should immediately terminate to receive the verdict <span class="tex-font-style-tt">Wrong answer</span>. Otherwise, it may receive any other verdict.</p><p>After outputting a query, do not forget to output an end of line and flush the output buffer. Otherwise, you will receive the verdict <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p>The interactor is <span class="tex-font-style-bf">non-adaptive</span>. The graph <span class="tex-font-style-bf">does not change</span> during the interaction.</p><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack, use the following format:</p><p>The first line contains a single integer $t$ ($1 \le t \le 1000$) ！ the number of test cases.</p><p>The only line of each test case contains a single integer $n$ ($2 \le n \le 10^5$) ！ the number of vertices in the graph.</p><p>Each of the following $(n - 2)$ lines should contains two integers $u$ and $v$ ($1 \le u, v \le n$, $u \ne v$) ！ ends of the edge that was removed from the graph. Each edge must not occur more than once.</p><p>The sum of $n$ over all test cases should not exceed $10^5$.</p></div>

## Input

<p>Each test consists of multiple test cases. The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. The description of the test cases follows.</p><p>The only line of each test case contains a single integer $n$ ($2 \le n \le 10^5$) ！ the number of vertices in the graph.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>





```input1
3
4

0 0

1 4

2 3

4

1 0

4 2

2

1 0
```




```output1
? 3

? 2

? 1

! 4 3 1 2

? 3

? 0

! 4 1 2 3

? 0

! 2 1
```



## Note

<p>In the first test case, the original graph looks as follows:</p><center> <img class="tex-graphics" src="./34706/file/WwfxfKde.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Consider the queries:</p><ul><li> There are no vertices with a degree of at least $3$ in the graph, so "$0\ 0$" is reported.</li><li> There are four vertices with a degree of at least $2$, and all of them have a degree of exactly $2$: $1$, $2$, $3$, $4$. Vertex $1$ is reported, because it has the minimum number, and vertex $4$ is reported, because it is the only one not connected to vertex $1$. After this, vertex $1$ is removed from the graph.</li><li> There are three vertices with a degree of at least $1$, among them vertices $2$ and $3$ have a minimum degree of $1$ (vertex $4$ has a degree of $2$). Vertex $2$ is reported, because it has the minimum number, and vertex $3$ is reported, because it is the only one not connected to vertex $2$. After this, vertex $2$ is removed from the graph.</li></ul><p>The path $4 - 3 - 1 - 2$ is a Hamiltonian path.</p><p>In the second test case, the original graph looks as follows:</p><center> <img class="tex-graphics" src="./34706/file/jIpOeBtP.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Consider the queries:</p><ul><li> Vertex $1$ has a degree of at least $3$, but it is connected to all vertices, so "$1\ 0$" is reported. After this, vertex $1$ is removed from the graph.</li><li> The remaining vertices $2$, $3$, and $4$ have a degree of at least $0$, but among them vertex $4$ has the minimum degree of $0$ (vertices $2$ and $3$ have a degree of $1$). Vertex $4$ is not connected to both vertices $2$ and $3$, so vertex $2$ is reported (as it has the minimum number). After this, vertex $4$ is removed from the graph.</li></ul><p>The path $4 - 1 - 2 - 3$ is a Hamiltonian path.</p><p>In the third test case, the graph consists of $2$ vertices connected by an edge.</p>
