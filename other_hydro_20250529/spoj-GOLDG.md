<p>Christian Goldbach sent a letter to Leonhard Euler in 1742 in which he made the following conjecture:</p>
<blockquote>
<p><em>"Every even number greater than 4 can be written as the sum of two odd prime numbers"</em></p>
</blockquote>
<p>To find the solutions of Goldbach's conjecture for a given even number <em>n</em> (<em>n </em>&gt; 0), let us define the directed graph GG(<em>n</em>) (the Goldbach Graph of <em>n</em>) as follows:</p>
<p>Nodes are prime numbers <em>p </em>such that 1 &lt; <em>p </em>&lt; <em>n</em>.<br>For each node <em>p</em> there are zero or more outgoing edges, determined by the following rules:<br>If <em>p </em>+ <em>q </em>= <em>n</em> and <em>q </em>= 1, then no outgoing edges are related to <em>p</em>.<br>If <em>p </em>+ <em>q </em>= <em>n</em> and <em>q </em>= <em>p</em><sub>1</sub> <em>p</em><sub>2</sub> <em>p</em><sub>3</sub> .... <em>p</em><sub>k</sub> is the prime factorization of <em>q</em> (asuming <em>q</em> &gt; 1), then for each <em>i </em>= 1..<em>k</em> an edge <em>p</em>-&gt;<em>p<sub>i</sub></em> is added to graph GG(<em>n</em>). Notice that each <em>p<sub>i</sub></em> must be a prime number. Besides, if <em>k </em>= 1 then <em>q</em> is prime and we have a solution to Goldbach's conjecture.</p>
<p><strong>For example:</strong></p>
<ul>
<li>GG(2) is empty (it has zero nodes)</li>
<li>GG(4) has two nodes and one edge.<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; nodes = {2, 3}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; edges = {2-&gt;2}</li>
<li>GG(6) has three nodes and three edges<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; nodes = {2, 3, 5}<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; edges = {2-&gt;2, 2-&gt;2, 3-&gt;3}<br>Notice that edge 2-&gt;2 appears twice in GG(6) because when <em>p</em> = 2 then <em>q</em> = 4 = 2*2</li>
</ul>
<p>Solutions to Goldbach's conjecture are cycles in graph GG(<em>n</em>) of the following types:</p>
<ul>
<li>Single-node cycles (Type I): a node <em>p</em> with only one outgoing edge <em>p</em>-&gt;<em>p</em>.</li>
<li>Double-node cycles (Type II): two nodes <em>p</em><sub>1</sub> and <em>p</em><sub>2</sub>, such that each one has a unique outgoing edge (<em>p</em><sub>1</sub>-&gt;<em>p</em><sub>2</sub>,<sub> </sub><em>p</em><sub>2</sub>-&gt;<em>p</em><sub>1</sub>).</li>
</ul>
<p>Your task is to inspect the directed graph GG(<em>n</em>) starting from a given node <em>x</em> and searching every node reachable from <em>x </em>for a solution to Goldbach's conjecture.&nbsp; The procedure is successfull if a node belonging to a Type I or Type II cycle is found. In such a case the minimum distance from<em> x</em> to the first node of the cycle found must be reported. Otherwise it should be stated that a solution can not be found.</p>
<p>Your algorithm should take into account that GG(<em>n</em>) can contain other types of cycles besides the ones described here. Otherwise, it can run forever.</p>
<h3>Input</h3>
<p>The input contains several lines each one with a different test case. Each line includes a pair of numbers representing the values <em>n</em> and <em>x</em>. You should assume that <em>n</em> is even and also that 2 &lt;= <em>n </em>&lt;= 1000. Although 0 &lt; <em>x </em>&lt; <em>n</em> is true, do not assume that <em>x</em> is a valid node of GG(<em>n</em>). The last line of the input contains the number 0 (it is not a test case).</p>
<h3>Output</h3>
<p>For each test case output a single line with one of the following:</p>
<ul>
<li>Solution found at distance <em>D</em>.</li>
<li>Solution not reachable.</li>
<li><em>x</em> is not a node!</li>
</ul>
<p>Where <em>D</em> is the minimum distance from <em>x</em> to the solution found, as described before.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<p style="padding-left: 30px;">2 1<br>4 2<br>6 2<br>6 3<br>12 3<br>12 11<br>14 7<br>20 5<br>38 11<br>50 17<br>540 340<br>540 31<br>540 33<br>0</p>
<pre><strong>Output:</strong></pre>
<p style="padding-left: 30px;">1 is not a node!<br>Solution found at distance 0.<br>Solution not reachable.<br>Solution found at distance 0.<br>Solution not reachable.<br>Solution not reachable.<br>Solution found at distance 0.<br>Solution found at distance 1.<br>Solution found at distance 2.<br>Solution found at distance 1.<br>340 is not a node!<br>Solution found at distance 0.<br>33 is not a node!</p>
<pre>&nbsp;</pre>