<p>The SUM problem can be formulated as follows: given four lists A, B, C, D  of integer values, compute how many quadruplet (a, b, c, d ) belongs to A x B x C x D  are such that a + b + c + d = 0 . In the following, we assume that all lists have the same size n 

</p><h3>Input</h3>
<p>
The first line of the input file contains the size of the lists n (this value can be as large as 4000). We then have n lines containing four integer values (with absolute value as large as 2<sup>28</sup> ) that belong respectively to A, B, C and D . 

</p><p>(<b>Edited: </b>n &lt;= 2500)</p>

<h3>Output</h3>
<p>Output should be printed on a single line.
</p><h3>Example</h3>
<pre><b>Input:</b>
6
-45 22 42 -16
-41 -27 56 30
-36 53 -37 77
-36 30 -75 -46
26 -38 -10 62
-32 -54 -6 45
<b>Output:</b>
5
</pre>