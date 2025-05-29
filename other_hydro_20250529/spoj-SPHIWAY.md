<p>There are N places and M bidirectional way. No two places have more than one direct way. Ana wants to walk from S to T and return to S by a itinerary that satisfy:</p>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; No way can be go twice.</p>
<p>-&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Length of itinerary is the minimum.</p>
<h3>Input</h3>
<p>Line 1: 4 integers: N, M, S, T (N &lt;= 10<sup>4</sup>; M &lt;= 10<sup>5</sup>)</p>
<p>Next M line: Line i include 3 integers u<sub>i</sub>, v<sub>i</sub>, c<sub>i</sub>: distance of two places u<sub>i</sub> and v<sub>i</sub> is c<sub>i</sub>. (c<sub>i</sub> &lt;= 2000000000).</p>
<h3>Output</h3>
<p>Length of the itinerary if it exists. Else print -1.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>5 7 1 5<br>1 2 3<br>1 4 8<br>2 3 5<br>2 4 4<br>3 5 5<br>4 3 8<br>4 5 3<br><br><strong>Output:</strong><br>24<br></pre>