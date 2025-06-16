<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MAXISET/en/">English</a></td> 
<td width="50%"><a href="/problems/MAXISET/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>You are given an unweighted undirected graph G. Each vertex has a positive weighted associated with it. Weight of a set of vertices is defined as the sum of weights of all vertices in the set.</p>
<p> A set of vertices is called independent if there is no edge in the graph with both endpoints on vertices of this set. </p>
<p>A subgraph induced by a set of vertices is a graph with vertex set as the given set of vertices and edges in the original graph with both endpoints in the given set.</p> 
<p>If s denotes a set of vertices, then Query(s, G) = Maximal weighted independent set in the subgraph induced by s. </p>
<p>Given q queries and the description of the graph, you are to output the weight of the Maximal weighted independent set corresponding to each of the queries. 
</p>
<h3>Input</h3>
<p>First line contains T, the number of test cases. </p>
<p>Each test case description starts with one line containing 2 integers n and m, denoting the number of vertices and number of edges. </p>
<p>Next line contains n space separated integers denoting the weight of vertices from 0 to n - 1 ( inclusive ). </p>
<p>Next m lines contains two integers u and v ( u != v, 0 ¡Ü u,v &lt; n ), denoting an undirected edge from u to v. </p>
<p>Next line contains q, the number of querries.</p>
<p> Next q lines contain description of a query. Description of a query starts with an integer denoting the size of set s, followed by the vertices which are members of vertex set s. </p>

<h3>Output</h3>
<p>For each test case, output q lines containing the answer to each query. Print a blank line BETWEEN the output of multiple test cases. </p>

<h3>Example</h3>

<pre><b>Input:</b>
2
5 1
1 2 3 4 5
0 1
3
3 0 1 2
3 1 2 3
2 0 1
3 3
1 2 3
0 1
0 2
1 2
1
3 0 1 2

<b>Output:</b>
5
9
2

3 
</pre>
<h3>Constraints</h3>
<p>
Dataset 1: T ¡Ü 20, n ¡Ü 30 , m ¡Ü 1000, q ¡Ü 1000 , weight_of_a_vertex ¡Ü 1000 Time limit: 5s   </p>
<p>
Dataset 2: T ¡Ü 10, n ¡Ü 40, m ¡Ü 1000, q ¡Ü 100, weight_of_a_vertex ¡Ü 1000 Time limit: 5s   
</p>