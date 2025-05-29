<p>Captain Claw is at the bank of a river of acid and he needs to cross it. Thr river is x metres wide but Captain Claw can jump at most d metres.</p>
<p>However, the Captain can jump only on stones which keep appearing in the stream.</p>
<h3><img title="River of Acid" src="./21847/file/XjJInBxW.png" alt="Captain Claw" width="585" height="202"></h3>
<h3>Input</h3>
<p>There are multiple test cases. For each test case.</p>
<p>The first line contains n,x and d.</p>
<p>The next n lines denotes subsequent seconds.</p>
<p>For each line, the first integer, c, denotes the number of number of stones appearing in this second.</p>
<p>Then c integers follow.</p>
<p>The ith integer means that a stone would appears at the position of that integer.</p>
<p>Find the minimum time needed by the Captain to cross the river.</p>
<p>1 &lt;= t &lt;= 30</p>
<p>1 &lt;= x &lt;= 10^5</p>
<p>1 &lt;= d &lt;=&nbsp; x</p>
<p>1 &lt;= n &lt;= 10^3</p>
<p>1 &lt;= sum(c) &lt;= 10^5</p>
<h3>Assumption</h3>
<p>Captain Claw is super fast . The time taken by jumps is negligible to a second.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print a single integer in each line - the time taken to cross the river.</p>
<p>Output -1 if its not possible to cross the river in n seconds.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>1<br>4 6 2<br>1 5<br>1 3<br>1 1<br>1 2<br><br><br><strong>Output:</strong><br>3<br><br></pre>
<p><strong>Explanation:</strong></p>
<p>Sec 1: Captain Waits</p>
<p>Sec 2: Captain Waits</p>
<p>Sec 3: Captain Jumps from bank(0) -&gt; 1 -&gt; 3 -&gt; 5 -&gt; bank(6)</p>
<h1><strong>&nbsp;</strong></h1>
<pre><strong>&nbsp;</strong></pre>