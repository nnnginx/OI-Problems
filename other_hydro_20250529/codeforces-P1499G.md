## Description

<div><p>You are given a bipartite graph consisting of $n_1$ vertices in the first part, $n_2$ vertices in the second part, and $m$ edges, numbered from $1$ to $m$. You have to color each edge into one of two colors, red and blue. You have to minimize the following value: $\sum \limits_{v \in V} |r(v) - b(v)|$, where $V$ is the set of vertices of the graph, $r(v)$ is the number of red edges incident to $v$, and $b(v)$ is the number of blue edges incident to $v$.</p><p>Sounds classical and easy, right? Well, you have to process $q$ queries of the following format:</p><ul> <li> $1$ $v_1$ $v_2$ ！ add a new edge connecting the vertex $v_1$ of the first part with the vertex $v_2$ of the second part. This edge gets a new index as follows: the first added edge gets the index $m + 1$, the second ！ $m + 2$, and so on. After adding the edge, you have to print the <span class="tex-font-style-it">hash</span> of the current optimal coloring (if there are multiple optimal colorings, print the <span class="tex-font-style-it">hash</span> of any of them). <span class="tex-font-style-bf">Actually, this hash won't be verified, you may print any number as the answer to this query, but you may be asked to produce the coloring having this hash</span>; </li><li> $2$ ！ print the optimal coloring of the graph with the same <span class="tex-font-style-it">hash</span> you printed while processing the previous query. The query of this type will only be asked after a query of type $1$, and there will be at most $10$ queries of this type. If there are multiple optimal colorings corresponding to this <span class="tex-font-style-it">hash</span>, print any of them. </li></ul><p>Note that if an edge was red or blue in some coloring, it may change its color in next colorings.</p><p>The <span class="tex-font-style-it">hash</span> of the coloring is calculated as follows: let $R$ be the set of indices of red edges, then the <span class="tex-font-style-it">hash</span> is $(\sum \limits_{i \in R} 2^i) \bmod 998244353$.</p><p>Note that you should solve the problem in <span class="tex-font-style-tt">online</span> mode. It means that you can't read the whole input at once. You can read each query only after writing the answer for the last query. Use functions <span class="tex-font-style-tt">fflush</span> in <span class="tex-font-style-tt">C++</span> and <span class="tex-font-style-tt">BufferedWriter.flush</span> in <span class="tex-font-style-tt">Java</span> languages after each writing in your program.</p></div><div class="input-specification"><p>The first line contains three integers $n_1$, $n_2$ and $m$ ($1 \le n_1, n_2, m \le 2 \cdot 10^5$).</p><p>Then $m$ lines follow, the $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i \le n_1$; $1 \le y_i \le n_2$) meaning that the $i$-th edge connects the vertex $x_i$ from the first part and the vertex $y_i$ from the second part.</p><p>The next line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of queries you have to process.</p><p>The next $q$ lines contain the queries in the format introduced in the statement.</p><p>Additional constraints on the input:</p><ul> <li> at any moment, the graph won't contain any multiple edges; </li><li> the queries of type $2$ are only asked if the previous query had type $1$; </li><li> there are at most $10$ queries of type $2$. </li></ul></div><div class="output-specification"><p>To answer a query of type $1$, print one integer&nbsp;！ the <span class="tex-font-style-it">hash</span> of the optimal coloring.</p><p>To answer a query of type $2$, print one line. It should begin with the integer $k$&nbsp;！ the number of red edges. Then, $k$ <span class="tex-font-style-bf">distinct</span> integer should follow&nbsp;！ the indices of <span class="tex-font-style-bf">red</span> edges in your coloring, in any order. Each index should correspond to an existing edge, and the <span class="tex-font-style-it">hash</span> of the coloring you produce should be equal to the <span class="tex-font-style-it">hash</span> you printed as the answer to the previous query.</p><p>If there are multiple answers to a query, you may print any of them.</p></div>

## Input

<p>The first line contains three integers $n_1$, $n_2$ and $m$ ($1 \le n_1, n_2, m \le 2 \cdot 10^5$).</p><p>Then $m$ lines follow, the $i$-th of them contains two integers $x_i$ and $y_i$ ($1 \le x_i \le n_1$; $1 \le y_i \le n_2$) meaning that the $i$-th edge connects the vertex $x_i$ from the first part and the vertex $y_i$ from the second part.</p><p>The next line contains one integer $q$ ($1 \le q \le 2 \cdot 10^5$)&nbsp;！ the number of queries you have to process.</p><p>The next $q$ lines contain the queries in the format introduced in the statement.</p><p>Additional constraints on the input:</p><ul> <li> at any moment, the graph won't contain any multiple edges; </li><li> the queries of type $2$ are only asked if the previous query had type $1$; </li><li> there are at most $10$ queries of type $2$. </li></ul>

## Output

<p>To answer a query of type $1$, print one integer&nbsp;！ the <span class="tex-font-style-it">hash</span> of the optimal coloring.</p><p>To answer a query of type $2$, print one line. It should begin with the integer $k$&nbsp;！ the number of red edges. Then, $k$ <span class="tex-font-style-bf">distinct</span> integer should follow&nbsp;！ the indices of <span class="tex-font-style-bf">red</span> edges in your coloring, in any order. Each index should correspond to an existing edge, and the <span class="tex-font-style-it">hash</span> of the coloring you produce should be equal to the <span class="tex-font-style-it">hash</span> you printed as the answer to the previous query.</p><p>If there are multiple answers to a query, you may print any of them.</p>

## Samples

```input1
3 4 2
1 2
3 4
10
1 1 3
1 2 3
2
1 3 3
2
1 2 4
2
1 2 1
1 1 1
2
```

```output1
8
8
1 3
40
2 3 5
104
3 5 6 3
104
360
4 5 6 3 8
```



