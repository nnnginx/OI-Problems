<p>Given an undirected graph with <strong>n</strong> nodes and <strong>m</strong> weighted edges, every node having one of two colors - black (denoted as 0) and white (denoted as 1). You are to perform <strong>q</strong> operations of two kinds:</p>
<ol type="1">
<li><strong>C</strong> x: Change the <em>x</em>-th node´s color. A black node should be changed into a white node, and vice versa. </li>
<li><strong>Q</strong> A B: Find the sum of weight of edges whose two end points of color A and B. A and B can be either 0 or 1.</li>
</ol>
<h3>Input</h3>
<p>The first line contains two integers <strong>n</strong> (1&lt;=<strong>n</strong>&lt;=10^5) and <strong>m</strong>(1&lt;=<strong>m</strong>&lt;= 10^5) specified above.</p>
<p>The second line contains <strong>n</strong> integers, the <em>i</em>-th of which represents the color of the <em>i</em>-th node, 0 for black and 1 for white.</p>
<p>The following <strong>m</strong> lines represent edges. Each line has three integer u, v and w(1&lt;=u, v&lt;=n, u!=v), indicating there is an edge of weight w between u and v. w fits into 32-bit signed integer.</p>
<p>The next line contains only one integer <strong>q</strong>(1&lt;=<strong>q</strong>&lt;= 10^5), the number of operations.</p>
<p>The following <strong>q</strong> lines - operations mentioned above. See samples for detailed format.</p>
<h3>Output</h3>
<p>For each <strong>Q</strong> query, print one line containing the desired answer.See samples for detailed format.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 3
0 0 0 0
1 2 1
2 3 2
3 4 3
4
Q 0 0
C 2
Q 0 0
Q 0 1
</pre>
<pre><strong>Output:</strong>
6
3
3
</pre>
<pre><strong>Input:</strong>
4 3
0 1 0 0
1 2 1
2 3 2
3 4 3
4
Q 0 0
C 3
Q 0 0
Q 0 1
</pre>
<pre><strong>Output:</strong>
3
0
4
</pre>
<p><strong>This problem has a somewhat strict source limit and time limit.</strong></p>