<p>You have a piece of iron wire with length of <strong>n</strong> unit. Now you decide to cut it into several ordered pieces and fold each piece into a triangle satisfying that all triangles are <strong>integral</strong> and pairwise <strong>similar</strong>.</p>
<p>count the number of different approaches to form triangles. Two approaches are considered different if they produce different numbers of triangles, and/or there exists <em>i</em> that the <em>i</em>-th (again, pieces are ordered) triangle in one approaches is not <strong>congruent</strong> to <em>i</em>th triangle in another plan.</p>
<p>Since the answer can be very large, output the answer modules 1000000007.</p>
<p><strong>Solve this problem by at most 0.5 KB of source code. </strong></p>
<h3>Input</h3>
<p>Each test case consists of one line containing one integer n (1&lt;=n&lt;=5,000,000). Process until EOF is reached.</p>
<h3>Output</h3>
<p>For each test case, output one line. See the example for more format details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
2
3
4
5
6
8
9
10
11
12
15
19
20
100
1000

<strong>Output:</strong>
Case 1: 0
Case 2: 0
Case 3: 1
Case 4: 0
Case 5: 1
Case 6: 2
Case 7: 1
Case 8: 6
Case 9: 3
Case 10: 4
Case 11: 10
Case 12: 25
Case 13: 10
Case 14: 16
Case 15: 525236
Case 16: 523080925
</pre>
<p><strong>Explanation</strong></p>
<p>A triangle is <strong>integral</strong> when all sides are integer.</p>
<p>Two triangles are <strong>congruent</strong> when all corresponding sides and interior angles are equal.</p>
<p>Two triangles are <strong>similar</strong> if they have the same shape.</p>
<p>For n = 9, there are 6 different ways: (1,1,1) * 3; (1,1,1), (2,2,2); (2,2,2),(1,1,1); (1,4,4); (2,3,4); (3,3,3).</p>