<p>Given a undirected graph with n veritces and m edges. Your taks is count the number of distinct pairs (u, v) that there is exist a path with length exactly 2 from u to v. Another mean, with each pair (u, v), we could find a vertex t that we have an edge (u, t) and (t, v). The input set may be contains multiple edge between any vertex and not consider to connected.</p>
<h3>Input</h3>
<p>- First line: n, m (1 &lt;= n, m &lt;= 10^5).</p>
<p>- m following line: u, v (1 &lt;= u, v &lt;= n).</p>
<h3>Output</h3>
<p>The number of distinct pairs.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 4<br>2 1<br>1 5<br>3 1<br>4 3<br><br><strong>Output:</strong>
4
<br><strong>Note: </strong>we have (1, 4), (2, 3), (2, 5), (3, 5)</pre>