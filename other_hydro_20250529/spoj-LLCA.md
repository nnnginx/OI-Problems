<p>Given a labeled complete k-ary tree, find the largest labeled common ancestor of two given nodes. In a complete k-ary tree, the node in the tree is labeled sequentially from the left most child to right most child, level by level. Largest labeled common ancestor of A and B is defined as the largest labeled node in the tree which has A and B as descendants. A node is a descendant of itself.</p>
<p><strong>Be careful with your finger, the source limit is 256 bytes.</strong></p>
<h3>Input</h3>
<p>The first line of input contains an integer T (1 &lt;= T &lt;= 100) the number of cases. Each cases contains three integers K, A and B (2 &lt;= K &lt;= 100; 1 &lt;= A,B &lt;= 2,000,000,000).</p>
<h3>Output</h3>
<p>For each test case, output in a line the largest labeled common ancestor node.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<br><br><br>4<br>3 42 7<br>2 2 6<br>2 1 105<br>4 10 13<br><br><strong>Output:</strong>
<br><br><br>2<br>1<br>1<br>3<br><br><strong>Whitespace Explanation:<br></strong>If there no input in any line, then the output for that line is a blank line :)) Sorry for inconvenience. &gt;:)</pre>