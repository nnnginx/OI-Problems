<p align="justify">You are given the coordinates of the vertices of a square in the 2-d plane. All vertex coordinates will be integers.</p>
<p align="justify">Now consider all convex quadrilaterals which also have integer coordinates for their vertices such that the midpoints of their edges are the vertices of the original square. Find the sum of areas of all such quadrilaterals.</p>
<h3>Input</h3>
<p align="justify">The first line of input gives T, the number of test cases (1¡ÜT¡Ü25000). Following this are the descriptions of the individual testcases. Each testcase consists of four lines, each line containing two space separated integers - the x and y coordinates of a distinct vertex of the square. The coordinate limits are -1000000000¡Üx<sub>i</sub>,y<sub>i</sub>¡Ü1000000000. It is assured that the four vertices will correspond to a square.</p>
<h3>Output</h3>
<p align="justify">For each testcase output the total area of quadrilaterals with the given property. Since the answer could be very large, give the answer modulo 100000007.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
0 0
1 1
1 0
0 1
0 1
1 0
0 -1
-1 0

<strong>Output:</strong>
0
4
</pre>