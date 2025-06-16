<p>You are given N (N &lt;= 100 000) d-dimensional (1 &lt;= d &lt;= 5) points, each having integer coordinates (X1, X2, ..., Xd). Then Q (Q &lt;= 100 000) queries follow. For each query you are given a d-dimensional point (not necessarily from the given N) and you are to find the squared Euclidean distance to the closest point from the given N.</p>
<p>The coordinates of all N+Q points are generated randomly between -1 000 000 000 and 1 000 000 000.</p>
<p>The squred Euclidean distance between two points A and B is the sum of (A.Xi-B.Xi)*(A.Xi-B.Xi) for i=1, 2, ..., d.</p>
<h3>Input</h3>
<p>The first line contains three numbers - N, d and Q.</p>
<p>The next N lines contain d integers each - the coordinates of a point.</p>
<p>The next Q lines contain d integers each - the coordinates of a query point.</p>
<h3>Output</h3>
<p>Print the answer for each of the Q queries on separate lines.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 56px; width: 1px; height: 1px; overflow: hidden;">2 2 2</div>2 2 2
1 1
2 2
1 1
3 3
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 56px; width: 1px; height: 1px; overflow: hidden;">1 1</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 56px; width: 1px; height: 1px; overflow: hidden;">2 2</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 56px; width: 1px; height: 1px; overflow: hidden;">3 3</div></pre>
<pre><strong>Output:</strong>
0
2</pre>