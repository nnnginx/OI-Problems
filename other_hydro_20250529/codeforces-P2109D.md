## Description

<div><p><span class="tex-font-style-it">Of course, a problem with the letter D is sponsored by Declan Akaba.</span></p><p>You are given a simple, connected, undirected graph with $n$ vertices and $m$ edges. The graph contains no self-loops or multiple edges. You are also given a multiset $A$ consisting of $\ell$ elements: $$ A = \{A_1, A_2, \ldots, A_\ell\} $$</p><p>Starting from vertex $1$, you may perform the following move <span class="tex-font-style-bf">any number</span> of times, as long as the multiset $A$ is not empty: </p><ul> <li> Select an element $k \in A$ and remove it from the multiset . You must remove exactly one occurrence of $k$ from $A$. </li><li> Traverse any walk$^{\text{∗}}$ of exactly $k$ edges to reach some vertex (possibly the same one you started from). </li></ul><p>For each $i$ ($1 \le i \le n$), determine whether there exists a sequence of such moves that starts at vertex $1$ and ends at vertex $i$, using the original multiset $A$. </p><p>Note that the check for each vertex $i$ is independent&nbsp;— you restart from vertex $1$ and use the original multiset $A$ for each case.</p><div class="statement-footnote"><p>$^{\text{∗}}$A walk of length $k$ is a sequence of vertices $v_0, v_1, \ldots, v_{k - 1}, v_k$ such that each consecutive pair of vertices $(v_i, v_{i + 1})$ is connected by an edge in the graph. The sequence may include repeated vertices.</p></div></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $m$, and $\ell$ ($2 \leq n \leq 2 \cdot 10^5$, $n-1 \leq m \leq 4 \cdot 10^5$, $1 \leq \ell \leq 2 \cdot 10^5$)&nbsp;— the number of vertices, the number of edges, and the size of the multiset, respectively.</p><p>The second line of each test case contains $\ell$ integers $A_1, A_2, \ldots, A_{\ell}$ ($1 \leq A_i \leq 10^4$)&nbsp;— the elements of the multiset.</p><p>Each of the following $m$ lines contains two integers $u$ and $v$ ($1 \le u &lt; v \le n$)&nbsp;— the endpoints of an edge in the graph. </p><p>It is guaranteed that the edges form a simple, connected graph without self-loops or multiple edges.</p><p>It is guaranteed that the sum of $n$, the sum of $m$, and the sum of $\ell$ over all test cases does not exceed $2 \cdot 10^5$, $4 \cdot 10^5$, and $2 \cdot 10^5$, respectively.</p></div><div class="output-specification"><p>For each test case, output a binary string of length $n$, where the $i$-th character is $\mathtt{1}$ if there exists a sequence of moves ending at vertex $i$, and $\mathtt{0}$ otherwise.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n$, $m$, and $\ell$ ($2 \leq n \leq 2 \cdot 10^5$, $n-1 \leq m \leq 4 \cdot 10^5$, $1 \leq \ell \leq 2 \cdot 10^5$)&nbsp;— the number of vertices, the number of edges, and the size of the multiset, respectively.</p><p>The second line of each test case contains $\ell$ integers $A_1, A_2, \ldots, A_{\ell}$ ($1 \leq A_i \leq 10^4$)&nbsp;— the elements of the multiset.</p><p>Each of the following $m$ lines contains two integers $u$ and $v$ ($1 \le u &lt; v \le n$)&nbsp;— the endpoints of an edge in the graph. </p><p>It is guaranteed that the edges form a simple, connected graph without self-loops or multiple edges.</p><p>It is guaranteed that the sum of $n$, the sum of $m$, and the sum of $\ell$ over all test cases does not exceed $2 \cdot 10^5$, $4 \cdot 10^5$, and $2 \cdot 10^5$, respectively.</p>

## Output

<p>For each test case, output a binary string of length $n$, where the $i$-th character is $\mathtt{1}$ if there exists a sequence of moves ending at vertex $i$, and $\mathtt{0}$ otherwise.</p>





```input1|2,3,4,5,6,7,8,16,17,18,19,20,21
3
6 5 2
2 3
1 2
2 3
3 4
4 5
5 6
5 5 1
5
1 2
2 3
3 4
4 5
3 5
5 4 3
100 200 300
1 2
1 3
1 4
2 5
```




```output1
111101
11111
10001
```



## Note

<p>In the first test case: </p><ul> <li> Vertex $1$ is reachable without making any moves. </li><li> Vertex $2$ is reachable by selecting element $3 \in A$; one possible walk is [$1 \rightarrow 2 \rightarrow 1 \rightarrow 2$]. </li><li> Vertex $3$ can be reached by selecting element $2 \in A$ and taking the walk [$1 \rightarrow 2 \rightarrow 3$]. </li><li> Vertex $4$ is reachable by selecting element $3 \in A$ and following the walk [$1 \rightarrow 2 \rightarrow 3 \rightarrow 4$]. </li><li> Vertex $5$ is not reachable by any valid sequence of moves. </li><li> Vertex $6$ is reachable by first selecting element $2 \in A$ and taking the walk [$1 \rightarrow 2 \rightarrow 3$], followed by selecting element $3 \in A$ and taking the walk [$3 \rightarrow 4 \rightarrow 5 \rightarrow 6$]. </li></ul>
