<p>A new planet full of rivers was discovered and is being prepared for colonization. We want to connect every piece of land by bridges, the cost of building a bridge is its width.</p>
<h3>Input</h3>
<p>The first number in the input file is T &lt; 200, the number of test cases. Each test case starts with a line with a integer, N &lt;= 500, the number of rivers. N lines are followed with 5 integers each, Di1, Fi1, Di2, Fi2 and Wi &lt;= 1000000, the coordinates of the extremities and the width of the i-th river. Every D is between -90 and 90, and every F is between 0 and 359, they are measured in degrees and correspond to the spherical coordinates (latitude and longitude respectively).<br>The two extremities of a river can be seen from above in a distance less than infinite, a course of a river is always the smallest possible and two rivers intersect in at most 1 point.</p>
<h3>Output</h3>
<p>For each test case print a single line with "Case #X: C" where X is the number of the test case (starting from 1) and C is the minimum cost to build the bridges so the islands and continents are connected directly or indirectly to each other.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br><br>3<br>4<br>0 0 90 0 4<br>90 0 0 179 2<br>0 0 -90 0 1<br>-90 0 0 179 1<br>6<br>0 0 10 90 3<br>0 0 -20 90 3<br>0 179 10 90 5<br>0 179 -20 90 1<br>0 0 0 179 10<br>-20 90 20 90 1<br>1<br>0 2 0 3 1

<strong>Output:</strong>
<br>Case #1: 1<br>Case #2: 6<br>Case #3: 0
</pre>