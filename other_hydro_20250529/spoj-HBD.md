<p><span style="font-size: small;">Today is problem setter's best friend Jenny¡¯s birthday. Long ago, Jenny, being a very clever girl, asked the problem setter to perform some queries on a tree but he couldn¡¯t do it. Now, he seeks your help to impress her on her birthday by answering those queries.</span></p>
<p><span style="font-size: small;">Recall that a tree is a connected acyclic undirected graph with <strong>n</strong> nodes and <strong>n-1</strong> edges. In each node there are some flowers. The two type of queries are described as:</span></p>
<p><strong><span style="font-size: small;">1 u v x</span></strong></p>
<p><strong><span style="font-size: small;">2 u y</span></strong></p>
<p><span style="font-size: small;">For first type, you have to calculate the minimum number of vertices needed to be visited on the path from <strong>v</strong> to <strong>u</strong>, starting at <strong>v</strong>, to collect at least <strong>x(1&lt;=x&lt;=1e18)</strong> flowers, where <strong>v</strong> is a descendant of <strong>u</strong>. <strong>Note that you cannot visit any node that is not in the path from v to u and you cannot skip any node of the path from v to that node you've chosen at last.</strong>&nbsp;If it's impossible to collect at least <strong>x</strong> flowers visiting all the vertices from <strong>v</strong> to <strong>u </strong>then you have to print <strong>-1</strong>.</span></p>
<p><span style="font-size: small;">For second type, you have to add y<strong>(y can be negative)</strong> to the existing amount flowers in node <strong>u</strong>. It is guaranteed that after this operation, flowers in a node will be non-negative and sum of flowers of all node of the tree will be at most 10^18.</span></p>
<p><span style="font-size: x-small;"><strong><span style="font-size: small;">Note that 1 is the root of the tree.</span></strong></span></p>
<h3><span style="font-size: medium;">Input</span></h3>
<p><span style="font-size: small;">The first line of the input contains two integers <strong>n</strong>(2 &lt;= n &lt;= 10^5) and <strong>q</strong>(1 &lt;= q &lt;= 10^5) where n is the number of vertices of the tree and q is the number of queries you have to perform.</span></p>
<p><span style="font-size: small;">Each of the next n-1 lines contains two integers <strong>a</strong>(1 &lt;= a &lt;= n) and <strong>b</strong>(1 &lt;= b &lt;= n) which denote an edge between a and b. The next line contains n non-negative integers c[1],c[2],..,c[n] (0 &lt;= c[i] &lt;= 10^13) where c[i] denotes the number of flowers in i¡¯th node. Next q lines contain queries of the format described above.&nbsp;</span></p>
<h3><span style="font-size: medium;">Output</span></h3>
<p><span style="font-size: small;">For each query of the first type print minimum number of nodes you have to visit to collect at least <strong>x</strong>(1 &lt;= x &lt;= 10^18) flowers. If it's impossible to collect at least <strong>x</strong> flowers visiting all the vertices from <strong>v</strong>&nbsp;to <strong>u</strong> then print <strong>-1</strong>.</span></p>
<h3><span style="font-size: medium;">Example</span></h3>
<pre><span style="font-size: small;"><strong>Input:</strong>
6 5
1 2
1 3
2 4
2 5
5 6
2 3 13 5 7 11
1 1 6 10
1 1 6 12
1 1 6 19
2 5 5
1 1 6 23</span></pre>
<pre><span style="font-size: small;"><strong>Output:</strong>
<strong>1</strong>
<strong>2</strong>
<strong>3</strong>
<strong>2</strong></span></pre>