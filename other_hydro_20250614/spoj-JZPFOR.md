<p>There are n lattice points in the 3D space. One point can get to another if and only if their euclid distance is 1. Find out the number of simple cycles (that has length &gt; 2). The number of points with same x coordinates do not exceed 8.&nbsp;</p>
<h3>Input</h3>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">First line, n.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Following are n lines, each describes one pointcoordinates.&nbsp;</div>
<p>First line, n.&nbsp;</p>
<p>Following are n lines, each describes one point, no two points share same coordinates.&nbsp;</p>
<p>n&lt;=400 &nbsp; &nbsp;coordinates in range [-10^9, 10^9] (inclusive).</p>
<h3>Output</h3>
<p>One number, the required answer mod 1000000007.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
8
0 0 0
0 0 1
0 1 0
0 1 1
1 0 0
1 0 1
1 1 0
1 1 1

<strong>Output:</strong>
28<span style="white-space: normal;">
</span></pre>