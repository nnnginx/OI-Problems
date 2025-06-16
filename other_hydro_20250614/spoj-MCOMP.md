<p style="text-align: justify;">Everyone knows what Manhattan streets look like. For simplicity, we'll say there are two types of streets: horizontal and vertical (when seen on a map). For two junctions A and B, with coordinates (ax, ay), (bx, by) respectively, we define distance( A, B ) = |ax-bx| + |ay-by|.</p>
<p style="text-align: justify;">A company in Manhattan has the following problem: we have to link N junctions by couriers in such a way that each pair of&nbsp; junctions can communicate through the couriers. We must use the minimal possible number of couriers to do so. Also, of all the possible solutions with the minimal number of couriers, we'll take the one that minimizes the maximum distance of assigned junction pairs over all the couriers.</p>
<h3>Input</h3>
<p>The first line of input contains a single integer: N (2 &lt;= N &lt;= 10<sup>5</sup>).<br>The next N lines each contains two integers: x<sub>i</sub> and y<sub>i</sub> (0 &lt;= x<sub>i</sub>, y<sub>i</sub> &lt;= 10<sup>5</sup>).</p>
<h3>Output</h3>
<p>The first and only line of output should contain the minimal maximum distance over all the couriers defined above.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>0 0<br>0 2<br>2 0<br><strong>Output:</strong>
2</pre>
<pre><strong>Explanation:</strong> couriers go between junction pairs ( 1, 2 ) and ( 1, 3 ). <br>Maximum distance is 2.</pre>