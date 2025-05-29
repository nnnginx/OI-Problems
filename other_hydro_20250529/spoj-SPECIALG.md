<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You are given a directed graph with N vertices. The special thing about the graph is that each vertex</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">has at most one outgoing edge. Your task is to answer the following two types of queries:</div>
<p>&nbsp;</p>
<h3><span style="font-size: 12px;">You are given a directed graph with N vertices. The special thing about the graph is that each vertex&nbsp;</span><span style="font-size: 12px;">has at most one outgoing edge. Your task is to answer the following two types of queries</span></h3>
<p><span style="font-size: small;">1 a  delete the only edge outgoing from vertex a. It is guaranteed that the edge exists. 1&lt;= a&lt;= N</span></p>
<p><span style="font-size: small;">&nbsp;</span></p>
<p><span style="font-size: small;">2 a b  output the length of the shortest path from vertex a to vertex b, if the path exists. Otherwise</span></p>
<p><span style="font-size: small;">output "-1" without quotes. 1&lt;=a, b&lt;= N</span></p>
<p>&nbsp;</p>
<h3><span style="font-size: small;">Input</span></h3>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong>First line of input contains a natural number N&lt;=10^5  the number of vertices in the graph.</strong></p>
<p><strong>The following line contains N integer numbers, i-th number is next[i] (0&lt;= next[i]&lt;= N), meaning that there</strong></p>
<p><strong>is an edge from vertex i to vertex next[i]. If next[i] = 0, assume that there is no outgoing edge from vertex</strong></p>
<p><strong>i.</strong></p>
<p><strong>Third line contains a natural number M&lt;=10^5  the number of queries.</strong></p>
<p><strong>The following M lines contain a query each. Queries are given in the manner described above.</strong></p>
<p>&nbsp;</p>
<h3><span style="font-size: medium;">Output</span></h3>
<p><span style="font-size: medium;"><span style="font-size: small;"> </span></span></p>
<p>On the i-th line output the answer for the i-th query of type 2 a b.</p>
<p><span style="font-size: 1.17em;">Example</span></p>
<p>&nbsp;</p>
<pre><strong>Input:</strong>
6
3 3 4 5 6 4
6
2 1 6
2 1 4
2 1 2
1 3
2 1 6
2 1 4

<strong>Output:</strong>
4
2
-1
-1
-1</pre>