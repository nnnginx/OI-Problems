<p>Given a graph G, and a subset of its vertices X. The associated cut of X is the set of edges<br>associated to X is the subset of all edges in G such that exactly one of the two vertices it joins<br>belongs to X.<br>In thinks, you will be given a graph and a subset of its edges, and you will have to determine<br>whether there exists a subset of the vertices of the graph for which the given subset of the edges<br>is its associated cut.</p>
<h3>Input</h3>
<p>The first line contains an integer T, the number of test cases (1 ¡Ü T ¡Ü 40). Each test case, consists of<br>a line which contains three integers N (2 ¡Ü N ¡Ü 500),E (1 ¡Ü E ¡Ü 104),K (1 ¡Ü K ¡Ü E), the number of<br>vertices in the graph, and the number of edges in the subset for which we want to know whether<br>it is an associated cut or not. Then, E lines follow, each of them contains two integers u,v (1 ¡Ü u,v ¡Ü<br>N) which are the vertices joined by the edge, the first K of these E lines represent the asked subset.</p>
<h3>Output</h3>
<p>Output T lines, one for each test case. If the asked subset is an associated cut, then print ¡°YES¡±,<br>otherwise print ¡°NO¡±.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br><br>3 3 1<br>1 2<br>2 3<br>1 3<br><br>12 17 6<br>3 4<br>5 6<br>10 11<br>1 5<br>6 10<br>4 8<br>1 2<br>2 3<br>6 7<br>7 8<br>9 10<br>11 12<br>5 9<br>2 6<br>3 7<br>7 11<br>8 12

<strong>Output:</strong>
NO<br>YES <br></pre>