<p>Given a N x M floor with few blocks already filled, check if it is possible to fill the remaining space with only 2 x 1 blocks, if it is not possible, print the minimum number of 1 x 1 blocks required to fill the floor&nbsp;completely.</p>
<h3>Input</h3>
<p>First line contains N (number of rows), M (number of columns), B (number of already blocked cells), followed by B lines each containing 2 integers x, y coordinates of the blocked cell</p>
<p>1 &lt;= N &lt;= 100, 1 &lt;= M &lt;= 100, 0 &lt;= B &lt;= N*M</p>
<h3>Output</h3>
<p>If it is possible to fill the floor with only 2 x 1 tiles, print Yes, else print No and the minimum number of 1 x 1 tiles required.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 1 0</pre>
<pre><strong>Output:</strong>
No 1</pre>
<pre><strong>Input:</strong></pre>
<pre>2 2 0</pre>
<pre><strong>Output:</strong></pre>
<pre><strong></strong>Yes</pre>
<pre><strong>Input:</strong></pre>
<pre><strong></strong>2 2 2</pre>
<pre>0 1</pre>
<pre>1 0</pre>
<pre><strong>Output:</strong></pre>
<pre><strong></strong>No 2</pre>