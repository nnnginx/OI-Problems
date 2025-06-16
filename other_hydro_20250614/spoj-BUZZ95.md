<p>You are given a sparse matrix of dimensions N x M. There K cells in the matrix {(x1,y1), (x2,y2), ..., (xK,yK)} with non-zero values {v1, v2, ..., vK}. All the other cells except these K cells contain value = 0. You are asked Q queries of the form sx sy fx fy, you need to print the sum of submatrix bounded by (sx,sy) and (fx,fy).</p>
<h3>Input</h3>
<p>First line contains two space separated integers N, M. (1 &lt;= N,M &lt;= 10^9)</p>
<p>Second line contains the integer K (1 &lt;= K &lt;= 10^5)</p>
<p>Next K lines contain three space separated integers xi, yi, vi. (1 &lt;= xi &lt;= N,1 &lt;= yi &lt;= M,1 &lt;= vi &lt;= 10^9).</p>
<p>Next line contains Q. (1 &lt;= Q &lt;= 10^5)</p>
<p>Next Q lines contain four space separated integers sx,sy,fx,fy. (1 &lt;= sx &lt;= fx &lt;= N,1 &lt;= sy &lt;= fy &lt;= M).</p>
<h3>Output</h3>
<p>For each query, print a single integer representing the sum of submatrix.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
10 10&nbsp;</pre>
<pre>2   </pre>
<pre>1 1 5   </pre>
<pre>2 2 15   </pre>
<pre>1    </pre>
<pre>1 1 3 3</pre>
<pre><strong>Output:</strong>
20</pre>