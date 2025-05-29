<p>Little Petar is playing a strategic warfare game against his opponent, Little Nikolaj. In the game, two players compete for supremacy over the opponent's base. The bases are located at the opposite ends of the map (Nikolaj's in the lower left corner of the map, Petar's in the upper right corner) and may be attacked or defended with the use of soldiers (that are at any time located at a given (x, y) coordinate pair on the map).</p>
<p>Petar has looked at Nikolaj's screen at a critical moment and successfully noted down all the positions where Nikolaj placed his soldiers, <strong>sorted in ascending order by the x coordinate</strong>. In order to plan an efficient attack, Petar is now interested in knowing how many of Nikolaj's soldiers are most vulnerable (i.e. located on the "frontline").</p>
<p>A soldier V(x, y) is <strong>located on the frontline</strong> if there is no other soldieimgr V'(x', y') such that x &lt;= x' and y &lt;= y', i.e. if there exists no other soldier that is "above-right" from that soldier.</p>
<h3>Input</h3>
<p>The first line of the standard input contains a natural number N, representing the number of Nikolaj's soldiers. Each of the following N lines contains two integers x<sub>i</sub> and y<sub>i</sub>, representing the coordinates of Nikolaj's i-th soldier. The soldiers will be sorted ascending by their x coordinate.</p>
<h3>Output</h3>
<p>Write to the standard output a single line containing the integer F, the number of Nikolaj's soldiers located on the frontline.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>6<br>0 1<br>1 5<br>3 5<br>3 2<br>4 4<br>5 1</pre>
<pre><strong>Output:</strong>
3
</pre>
<h3>Explanation</h3>
<p>The positions of Nikolaj's soldiers from the given testcase are shown on the image below. The frontline is marked with the red line and consists of the following set of soldiers: {(3, 5), (4, 4), (5, 1)}.</p>
<p><img src="../../../../../../content/simes:FRONT.png" alt="Front" width="300" height="301"></p>
<h3>Constraints</h3>
<ul>
<li>1 &lt;= N &lt;= 10<sup>6</sup></li>
<li>0 &lt;= x<sub>i</sub>, y<sub>i</sub> &lt;= 10<sup>9</sup></li>
<li>No pair of soldiers will share the same position.</li>
<li>The soldiers will be sorted ascending by their x coordinate, i.e. x<sub>1</sub> &lt;= x<sub>2</sub> &lt;= ... &lt;= x<sub>N</sub>.</li>
</ul>