<p>Most of the traffic accidents occur at road intersections. In order to deal with the traffic accidents efficiently, the traffic police should arrive at the accidental scene quickly. You, as an urban planner, are entrusted to select the best location in the urban area to build the traffic police station.</p>
<p>You are given <strong>N</strong> coordinates <strong>(X<sub>i</sub>, Y<sub>i</sub>, Z<sub>i</sub>)</strong>, where X, Y describe the 2D position and Z is&nbsp; the height of terrain, representing those road intersections that always have traffic accidents. To simplify the problem, best location means a given road intersection(s) that minimizes the sum of distances to all other given intersections. That is, you will choose a given road intersection(s) as potential location to build the station. Please note that the traffic police can only move along the road horizontally and vertically, but not diagonally which will be blocked by buildings. The length of each street block is 1, and all roads are connected in grid pattern.</p>
<h3>Input</h3>
<p>The first line of input is the number of test cases <strong>T</strong>. (1 ¡Ü&nbsp;T ¡Ü&nbsp;50)</p>
<p>For each test case, the first line is the numbers of road intersections that always have traffic accidents <strong>N</strong>. (1 ¡Ü&nbsp;N ¡Ü&nbsp;1000)</p>
<p>The following N lines are the coordinates of each road intersection <strong>X</strong><sub>i</sub><strong> Y</strong><sub>i</sub><strong> Z</strong><sub>i</sub>. (-1000 ¡Ü&nbsp;X<sub>i</sub>, Y<sub>i</sub>&nbsp;Z<sub>i</sub><sub>&nbsp;</sub>¡Ü&nbsp;1000)</p>
<p>It is guaranteed that no coordinates are duplicate.</p>
<h3>Output</h3>
<p>For each test case, output the coordinates <strong>X Y Z</strong> of selected road intersection(s) to build the traffic police station. If there is more than one best location, output all of them according to the input order line by line.</p>
<p>After each test case, print a blank line.</p>
<h3>Example</h3>
<pre><strong>Input: </strong>
2

7
2 6 3
1 -5 0
-100 -10 3
3 3 3
0 150 9
999 -3 0
878 123 4

2
-5 -10 0
0 -10 0

</pre>
<pre><div id="_mcePaste" style="position: absolute; left: -10000px; top: 226.4px; width: 1px; height: 1px; overflow: hidden;">0 -10 0</div><strong>Output:</strong>
3 3 3

-5 -10 0
0 -10 0

</pre>