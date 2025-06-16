<p>Count the number of rooted trees with n nodes, which satiesfy the following condition:</p>
<p>If the distance between node A and the root equals to the distance between node B and the root, then A and B must have same number of (direct) children.</p>
<p>Two trees are considered identical if and only if there's a bijection of n nodes which transforms one tree into another one.</p>
<p>Since the answer can be very large, output the answer modules 1000000007.</p>
<h3>Input</h3>
<p>Each test case consists of one line containing one integer n (1&lt;=n&lt;=1000). Process until EOF is reached.</p>
<h3>Output</h3>
<p>For each test case, output one line. See the example for more format details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
2
3
40
50
600
700

<strong>Output:</strong>
Case 1: 1
Case 2: 1
Case 3: 2
Case 4: 924
Case 5: 1998
Case 6: 315478277
Case 7: 825219749
</pre>