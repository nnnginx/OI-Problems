<h3>Problem</h3>
<p align="justify">
K-path cover of a directed graph is a set of exactly k of its edges chosen in such way that every two of them have different start vertices and every two of them have different end vertices. Assuming that for each vertex we know its cost we can define cost of the edge as a sum of costs of its start and end. We can also define cost of a k-path cover as a sum of costs of its edges. Your task is to find cheapest k-path cover for given directed graph with known costs of the vertices.
</p><center>
<img src="/content/gawry:cover.gif"><br>
A graph and its cheapest 4-path cover.
</center>
<p></p>
<h3>Input</h3>
<p align="justify">
First line of input contains number of test cases c (1&lt;=c&lt;=20). Each test case begins with k, number of vertices n and number of edges m (1&lt;=k&lt;=100, 1&lt;=n&lt;=10000, 0&lt;=m&lt;=1000000). Next n lines contain costs of the vertices, each of them is an integer from [-100000,100000]. Then m lines describing edges follow, each of them containing exactly two numbers representing its start and end vertices. Vertices are numbered from 1 to n.
</p>
<h3>Output</h3>
<p align="justify">
For each test case output cost of the cheapest k-path cover. When given graph has no k-path cover output NONE.
</p>
<h3>Example</h3>
<pre>Input:
1
4 6 9
5
4
6
10
2
3
1 2
1 4
2 4
3 2
4 3
5 4
6 3
5 6
6 5

Output:
33
</pre>