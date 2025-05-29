<p>Let Lx denote the level of a node x in a rooted tree. Lx is 1 if x is the root, otherwise Lx = 1 + Ly, where y is the parent of x in the rooted tree.</p>

<p>You need to calculate the sum Lx ^ K for all nodes x in the tree.</p>

<h3>Input</h3>
<p>The first line contains the number of test cases T. T test cases follow. The first line of each test case contains N and K, where N is the number of nodes in the tree. The following N - 1 lines contain two integers ai and bi, indicating an edge between nodes ai and bi in the tree. There is a blank line after each test case.

</p><h3>Output</h3>
<p>Output N lines for each test case. The i-th line should contain the required sum if the tree is rooted at node i. Output all values modulo 1000000007. Output a blank line after each test case.
</p>

<h3>Example</h3>
<pre><strong>Sample Input:</strong>
2
3 2
0 1
1 2

3 3
0 1
0 2

<b>Sample Output:</b>
14
9
14

17
36
36</pre>

<h3>Constraints</h3>
<p>1 &lt;= T &lt;= 10<br>1 &lt;= N &lt;= 20000<br>1 &lt;= K &lt;= 20<br>0 &lt;= ai, bi &lt; N</p>