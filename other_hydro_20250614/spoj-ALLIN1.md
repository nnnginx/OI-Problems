<p><em>Before you begin, you should try this problem! <a href="../SDITSAVL/">AVL Tree</a></em></p>
<p>This problem is simple. Initially, there is a list and it's empty. Then you are given four types of query.</p>
<ol>
<li>Insert data to the list</li>
<li>Remove data from the list</li>
<li>Print an index (1-based) from a specified data after the list was sorted ascendingly</li>
<li>Print data from a specified index (1-based) after the list was sorted ascendingly</li>
</ol>
<h3>Input</h3>
<p>Input contains several lines. Each line follows one of these formats.<br><strong>1 n</strong>: Insert <strong>n</strong> (0 &lt;= n &lt;= 2<sup>31</sup> - 1) to the list<br><strong>2 n</strong>: Remove <strong>n</strong> from the list. If <strong>n</strong> was not found, do nothing<br><strong>3 n</strong>: Print <strong>n</strong>'s index (1-based) after the list was sorted ascendingly<br><strong>4 i</strong>: Print data on <strong>i</strong>-th index (1-based) after the list was sorted ascendingly (0 &lt;= i &lt;= 2<sup>31</sup> - 1)<br><strong>-1</strong>: End of input</p>
<h3>Output</h3>
<p>For each query 3, print <strong>n</strong>'s index in one line. If <strong>n</strong> was not found, just print -1<br>For each query 4, print data on <strong>i-</strong>th index in one line. If the index is not valid, just print -1</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 20<br>-1

<strong>Output:</strong>
-1<br>&nbsp;</pre>