<p>It's a cruel war which kills millions of people and series of cities were ruined. In order to stop it, let's bomb the opponent's base.</p>
<p>It seems to be not a hard work in circumstances of street battles, however, you'll be encountered a much more difficult instance: recounting exploits of the military. In the bombing action, the commander will dispatch a group of bombers with weapons having the huge destructive power to destroy all the targets in a line. Thanks to the outstanding work of our spy, the positions of all opponents' bases had been detected and marked on the map, consequently, the bombing plan will be sent to you.</p>
<p>Specifically, the map is expressed as a 2D-plane with some positions of enemy's bases marked on. The bombers are dispatched orderly and each of them will bomb a vertical or horizontal line on the map. Then your commanded wants you to report that how many bases will be destroyed by each bomber. Notice that a ruined base will not be taken into account when calculating the exploits of later bombers.</p>
<h3>Input</h3>
<p>Multiple test cases. Each test cases starts with two non-negative integer <strong>N</strong> (<strong>N</strong> &lt;= 100,000) and <strong>M</strong> (<strong>M</strong> &lt;= 100,000) denoting the number of target bases and the number of scheduled bombers respectively. In the following <strong>N</strong> line, there is a pair of integers separated by single space indicating the coordinate of position of each opponent's base. The following <strong>M</strong> lines describe the bombers, each of them contains two integers <strong>c</strong> and <strong>d</strong> (0&lt;= <strong>c</strong> &lt;=1 , -1,000,000,000 &lt;= <strong>d</strong> &lt;= 1,000,000,000). <strong>c</strong> = 0 means this bomber will bomb the line x = <strong>d</strong>, <strong>c</strong> = 1 means this bomber will bomb the line y = <strong>d</strong>.</p>
<p>The input ends with <strong>N</strong> = <strong>M</strong> = 0.</p>
<h3>Output</h3>
<p>For each test case, output <strong>M</strong> lines, the <em>i</em>-th line contains a single integer denoting the number of bases that were destroyed by the corresponding bomber in the input. Output a blank line after each test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 2
1 2
1 3
2 3
0 1
1 3
0 0

<strong>Output:</strong>
2
1
</pre>
<b>Warning: large input/output data, be careful with certain languages</b>