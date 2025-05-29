<p>Mr. B, Mr. G, Mr. M and their coach Professor S are planning their way to Warsaw for the ACM-ICPC World Finals. Each of the four has a square-shaped suitcase with side length A<sub>i</sub> (1 &lt;= <em>i</em> &lt;= 4) respectively. They want to pack their suitcases into a large square box. The heights of the large box as well as the four suitcases are exactly the same. So they only need to consider the large box¡¯s side length. Of course, you should write a program to output the minimum side length of the large box so that the four suitcases can be put into the box without overlapping.</p>
<h3>Input</h3>
<p>Each test case contains only one line containing 4 integers A<sub>i</sub> (1&lt;= <em>i</em> &lt;=4, 1&lt;= A<sub>i</sub> &lt;=1,000,000,000) indicating the side length of each suitcase.</p>
<h3>Output</h3>
<p>For each test case, display a single line containing the case number and the minimum side length of the large box required.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 2 2 2
2 2 2 1

<strong>Output:</strong>
Case 1: 4
Case 2: 4
</pre>
<p><strong>Explanation<strong> </strong></strong></p>
<p>For the first case, all suitcases have size 2x2. So they can perfectly be packed in a 4x4 large box without wasting any space.</p>
<p>For the second case, three suitcases have size 2x2 and the last one is 1x1. No matter how to rotate or move, you could find the side length of the box must be at least 4.</p>