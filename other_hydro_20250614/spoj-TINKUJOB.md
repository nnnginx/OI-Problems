<p>Tinku has a new job at BIT. The job pays well, and provides Tinku  with a house to live within BIT. His only job is to deliver goods to  Main Building. The goods are to be collected from a pickup point.  Therefore, a typical day of work for Tinku begin with him leaving his  home, collecting the goods from the pickup point, and ends with him  delivering the goods to the Main Building. Pickup points are arbitrary  locations in the BIT campus.</p>
<p>The whole BIT campus can be represented as a 2-D plane. Tinku's House, Main Building and pickup points can only be present at <strong>integer coordinates</strong>. You are given the coordinates of Tinku's house and the Main Building (<strong>See the input format carefully</strong>). The distance considered is the euclidean distance, i.e, distance from point (a, b) to (c, d) will be sqrt((a-c)^2 + (b-d)^2). A main building can also be a pickup point.</p>
<p>The job contract ensures that Tinku works <strong>atmost for H hours</strong>.  Tinku is new at this job, and is very nervous. ACM people being  friendly as always, decide to ease him up by finding the number of  possible pickup points such that Tinku is able to finish his work.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line denotes number of test cases T<br>T test cases follow<br>Each test case is formatted as:<br>First line consist of integers A, B, C, H, V<br>Tinku's house is at coordinate (A, C), and Main Building is at (B, C)<br>Tinku works at most for H hours and has walks with a speed of V units/hour</p>
<p><code>T = 1000</code><br><code>-100 &lt;= A, B, C &lt;= 100</code><br><code>0 &lt; V &lt;= 40</code><br><code>0 &lt; H &lt;= 40</code></p>
<h3>Output</h3>
<p>A single line with the number of possible pickup points</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<code>2<br>1 -1 0 1 3<br>-5 5 10 2 2</code>

<strong>Output:</strong>
<code>5</code><br><code>0</code>
</pre>