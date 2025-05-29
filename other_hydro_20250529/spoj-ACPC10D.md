<p>Here¡¯s a simple graph problem: Find the shortest path from the top-middle vertex to the bottom-middle vertex in a given tri-graph. A tri-graph is an acyclic graph of (N ¡Ý 2) rows and exactly 3 columns. Unlike regular graphs, the costs in a tri-graph are associated with the vertices rather than the edges.</p>
<p style="text-align: center;"><img title="a" src="../../../content/omar_azazy:ACPC10D" alt="a" width="271" height="405"></p>
<p>So, considering the example with N = 4, the cost of going straight down from the top to bottom along the middle vertices is 7 + 13 + 3 + 6 = 29. The layout of the directional edges in the graph are always the same as illustrated in the figure.</p>
<h3>Input</h3>
<p>Your program will be tested on one or more test cases.<br>Each test case is specified using N + 1 lines where the first line specifies a single integer (2 ¡Ü N ¡Ü 100, 000) denoting the number of rows in the graph. N lines follow, each specifying three integers representing the cost of the vertices on the ith row from left to right. The square of each cost value is less than 1,000,000.<br>The last case is followed by a line with a single zero.</p>
<h3>Output</h3>
<p>For each test case, print the following line:<br>k. n<br>Where k is the test case number (starting at one,) and n is the least cost to go from the top-middle vertex to the bottom-middle vertex.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>4<br>13 7 5<br>7 13 6<br>14 3 12<br>15 6 16<br>0<br><br><strong>Output:</strong><br>1. 22</pre>