<p>There is a regular n-gon. We mark some points on its sides: a1 points on the first side, a2 on the second ... an on the last. Marked points do not coincide with the vertices n-gon. The question is, how many different convex nondegenerate (n-1)-gons you can build, using marked points as vertices?

</p><h3>Input</h3>
<p>The first line of input contains the number t - the number of tests. Next comes the description of t tests. Each test consists of two lines. The first line of the test contains an integer n - number of vertices of original n-gon. Second line of the test lists n integers a1, a2, ..., an - number of points marked on each side.

</p><h3>Constraints</h3>
<p>1 &lt;= t &lt;= 20<br>
4 &lt;= n &lt;= 1000<br>
1 &lt;= ai &lt;= 100

</p><h3>Output</h3>
<p>For each test, print out the answer to the problem modulo 1000000007.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
4
2 2 2 2
5
2 2 2 2 2
5
10 20 30 40 50

<b>Output:</b>
56
210
16207125

</pre>