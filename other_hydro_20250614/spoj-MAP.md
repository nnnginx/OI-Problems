<p>
After a new administrative division of Byteland cartographic office works on a
new demographic map of the country. Because of technical reasons only
a few colors can be used. The map should be colored so that regions with the same or similar
population (number of inhabitants) have the same color. For a given color<i> k</i> let
<b>A</b>(<i>k</i>) be the number, such that:&nbsp;

</p><ul>
<li>at least half of regions with color <i> k</i> has population not greater than
  <b>A</b>(<i>k</i>)
</li><li>at least half of regions with color <i> k</i> has population not less than <b>A</b>(<i>k</i>)&nbsp;
</li></ul>

<p><b>A coloring error of a region</b> is an absolute value of the difference between
<b>A</b>(<i>k</i>) and the region's population.
<b>A cumulative error</b> is a sum of coloring errors of all regions. We are
looking for an optimal coloring of the map (the one with the minimal cumulative
error).</p>

<h3>Task</h3>
<p>Write a program which:
</p><ul>
<li>reads the population of regions in Byteland from the standard input,
</li><li>computes the minimal cumulative error,
</li><li>writes the result to the standard output.
</li></ul>

<h3>Input</h3>
<p>
The number of test cases t is in the first line of input, then t test cases follow separated by an empty line.
In the first line of each test case an integer <i>n</i> is written, which is the number of regions in
Byteland, <i> 10&lt; n &lt;3000</i>. In the second line the number <i>m</i>
denoting the<i> </i>number of colors used to color the map is written, <i> 2 &lt;= m &lt;= 10</i>. In each
of the following <i> n</i> lines there is one non-negative integer - a
population of one of the regions of Byteland. No population exceeds <i>2^30</i>.&nbsp;
</p>

<h3>Output</h3>
<p>
Your program should write for each test case one integer number equal to a minimal
cumulative error, which can be achieved while the map is colored (optimally).
</p>

<h3>Example</h3>

<pre><b>Sample input:</b>
1
11
3
21
14
6
18
10
2
15
12
3
2
2

<b>Sample output:</b>
15
</pre>