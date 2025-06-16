<p>Consider two arbitrarily chosen horizontal lines. A trapezoid Ti between these lines has two<br>vertices situated on the upper line and the other two vertices on the lower line (see figure below).<br>We will denote by ai, bi, ci and di the upper left, upper right, lower left and respectively lower right<br>vertices of the trapezoid Ti. A subset S of trapezoids is called independent if no two trapezoids from<br>S intersect.</p>
<h3>Task</h3>
<p>Determine the cardinality of the largest independent set of trapezoids (the largest set means the set<br>with most elements). Also find the count of different independent sets with maximum cardinality.<br>Find this count modulo 30013.</p>
<h3>Input</h3>
<p>The first line of input contains one integer N ¨C the number of trapezoids. Each of the next N lines<br>contains four integers ai, bi, ci and di. No two trapezoids have a common vertex (corner).</p>
<h3>Output</h3>
<p>The only line of output should contain two numbers separated by space: firstly, the cardinality of<br>the largest independent set; secondly, the count of different independent sets with maximum<br>cardinality modulo 30013.</p>
<h3>Constraints</h3>
<p>1 ¡Ü N ¡Ü 100 000<br>1 ¡Ü ai, bi, ci, di ¡Ü 1 000 000 000</p>
<h3>Example</h3>
<p>The picture below is NOT an accurate representation. The trapezoids' top and bottom have been shifted up and down for visibility.</p>
<p><img title="Trapezoid" src="../../../content/simes:TRAPEZBO.png" alt="Trapezoid_Example" width="544" height="92"></p>
<pre><strong>Input:</strong>
7<br>1 3 1 9<br>4 7 2 8<br>11 15 4 12<br>10 12 15 19<br>16 23 16 22<br>20 22 13 25<br>30 31 30 31

<strong>Output:</strong>
<br>3 8</pre>