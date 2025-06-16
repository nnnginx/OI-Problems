<p>You are given a bipartite graph with N(1&lt;=N&lt;=300) nodes on each side.         Determine whether the number of perfect matching is odd or even.</p>
<h3>Input</h3>
<p>First line is an integer T(1&lt;=T&lt;=20) means the number of test  cases. 	The following are T parts. 	Each part begin with an integer N(1&lt;=N&lt;=300) means the number of  nodes on both sides. 	It followed with N lines, each line contains a 0/1 string. 	If the j(1&lt;=j&lt;=N)th character of the i(1&lt;=i&lt;=N)th line is  1, it means the i th node on left have an edge to the j th node on  right. 	See the sample for details.</p>
<h3>Output</h3>
<p>T lines, each contain "Odd" or "Even", which means the parity of the number of the perfect matching. 	See the sample for details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2   <br>1<br>1<br>4<br>1100<br>1100<br>0011<br>0011<br><strong>Output:</strong>
Odd<br>Even<br><br></pre>
<h3>Constraints</h3>
<p>1 &lt;=N &lt;= 300<br>1 &lt;=T &lt;= 20</p>