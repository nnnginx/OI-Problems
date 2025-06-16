<p>Little Gopu was playing with graphs. He encoutered following problem while playing.</p>
<p>Given a graph G with n vertices and m edges. Let us say it has k connected components. Find out how many numbers of ways you can add k - 1 edges to make the graph connected. Note that the new edge you are going to add should not be a repeated edge ie. if you are going to connect u, v then there should not be an edge between u, v already in the graph. Output the answer modulo 10^9 + 7.</p>
<p>If the graph is already connected, Output -1</p>
<p>Help Gopu with this task.</p>
<h3>Input</h3>
<p>First line contains T : number of test cases. (1 &lt;= T &lt;= 20)</p>
<p>For each test case, First line contains two space seperated integers n, m: (1 &lt;= n, m &lt;= 10^5).</p>
<p>Then For each of the next m lines, each line contains two space seperated integers u and v denoting that u and v are connected to each other. (1 &lt;= u, v &lt;= n and u != v) &nbsp;</p>
<h3>Output</h3>
<p>For each test case, output the answer as required.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4<br>4 2<br>1 2<br>3 4<br>5 3<br>1 2<br>3 4<br>4 5<br>3 3<br>1 2<br>2 3<br>3 1<br>7 5<br>1 2<br>3 4<br>4 5<br>3 5<br>6 7&nbsp;</pre>
<pre><strong>Output:</strong>
4<br>6<br>-1<br>84</pre>