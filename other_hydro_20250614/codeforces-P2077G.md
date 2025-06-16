## Description

<div><div class="epigraph"><div class="epigraph-text"><span class="tex-font-style-it"><a href="https://www.youtube.com/watch?v=UeN7U474cxE">Red and Blue and Green - fn and Silentroom</a></span></div><div class="epigraph-source">⠀</div></div><p>You are given a connected graph with $n$ vertices and $m$ bidirectional edges with weight not exceeding $x$. The $i$-th edge connects vertices $u_i$ and $v_i$, has weight $w_i$, and is assigned a color $c_i$ ($1 \leq i \leq m$, $1 \leq u_i, v_i \leq n$). The color $c_i$ is either red, green, or blue. It is guaranteed that there is <span class="tex-font-style-bf">at least</span> one edge of each color.</p><p>For a walk where vertices and edges may be repeated, let $s_r, s_g, s_b$ denote the sum of the weights of the red, green, and blue edges that the walk passes through, respectively. If an edge is traversed multiple times, each traversal is counted separately.</p><p>Find the minimum value of $\max(s_r, s_g, s_b) - \min(s_r, s_g, s_b)$ over all possible walks from vertex $1$ to vertex $n$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $m$, and $x$ ($4 \leq n \leq 2 \cdot 10^5$, $n-1 \leq m \leq 2 \cdot 10^5$, $1 \leq x \leq 2 \cdot 10^5$)&nbsp;— the number of vertices, the number of edges in the graph, and the upper bound on the weight of the edges, respectively.</p><p>The next $m$ lines each contain three integers $u_i, v_i, w_i$ and a letter $c_i$ ($1 \leq u_i, v_i \leq n$, $1 \leq w_i \leq x$), representing a bidirectional edge between vertices $u_i$ and $v_i$ with weight $w_i$ and color $c_i$. The color $c_i$ is either 'r', 'g', or 'b', denoting red, green, and blue, respectively.</p><p>It is guaranteed that the graph is connected and contains at least one edge of each color. The graph may also contain <span class="tex-font-style-bf">multiple</span> edges and <span class="tex-font-style-bf">self-loops</span>.</p><p>Additionally, it is guaranteed that the total sum of all values of $n$, the total sum of all values of $m$, and the total sum of all values of $x$ across all test cases do not exceed $2 \cdot 10^5$ individually.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;— the minimum value of $\max(s_r, s_g, s_b) - \min(s_r, s_g, s_b)$ over all walks from vertex $1$ to vertex $n$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $m$, and $x$ ($4 \leq n \leq 2 \cdot 10^5$, $n-1 \leq m \leq 2 \cdot 10^5$, $1 \leq x \leq 2 \cdot 10^5$)&nbsp;— the number of vertices, the number of edges in the graph, and the upper bound on the weight of the edges, respectively.</p><p>The next $m$ lines each contain three integers $u_i, v_i, w_i$ and a letter $c_i$ ($1 \leq u_i, v_i \leq n$, $1 \leq w_i \leq x$), representing a bidirectional edge between vertices $u_i$ and $v_i$ with weight $w_i$ and color $c_i$. The color $c_i$ is either 'r', 'g', or 'b', denoting red, green, and blue, respectively.</p><p>It is guaranteed that the graph is connected and contains at least one edge of each color. The graph may also contain <span class="tex-font-style-bf">multiple</span> edges and <span class="tex-font-style-bf">self-loops</span>.</p><p>Additionally, it is guaranteed that the total sum of all values of $n$, the total sum of all values of $m$, and the total sum of all values of $x$ across all test cases do not exceed $2 \cdot 10^5$ individually.</p>

## Output

<p>For each test case, output a single integer&nbsp;— the minimum value of $\max(s_r, s_g, s_b) - \min(s_r, s_g, s_b)$ over all walks from vertex $1$ to vertex $n$.</p>





```input1|2,3,4,5,12,13,14,15,16,17,18
3
4 3 3
1 2 2 r
2 3 3 g
3 4 2 b
4 5 4
1 2 1 r
1 1 1 r
2 1 1 r
2 3 4 g
3 4 4 b
4 6 4
1 2 2 r
1 2 2 r
2 3 3 b
1 3 4 r
1 4 1 g
3 4 4 g
```




```output1
1
0
0
```



## Note

<p>In the first test case, the optimal path is $1 \to 2 \to 3 \to 4$. The edges used are: </p><ul> <li> $1 \to 2$ (red, weight $2$) </li><li> $2 \to 3$ (green, weight $3$) </li><li> $3 \to 4$ (blue, weight $2$) </li></ul><p>We have $s_r = 2$, $s_g = 3$, and $s_b = 2$. Thus, the answer is $1$.</p><p>In the second test case, one of the optimal paths is $1 \to 1 \to 2 \to 1 \to 2 \to 3 \to 4$. The edges used are: </p><ul> <li> $1 \to 1$ (red, weight $1$) </li><li> $1 \to 2$ (red, weight $1$) </li><li> $2 \to 1$ (red, weight $1$) </li><li> $1 \to 2$ (red, weight $1$) </li><li> $2 \to 3$ (green, weight $4$) </li><li> $3 \to 4$ (blue, weight $4$) </li></ul><p>We have $s_r = s_g = s_b = 4$. Thus, the answer is $0$.</p>
