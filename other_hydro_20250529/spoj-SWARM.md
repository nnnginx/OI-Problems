<p>There is a regular n-gon. Some points are marked on each of its sides. There are x<sub>1</sub> point marked on the first side, x<sub>2</sub> �C on the second, ��, x<sub>n</sub> �C on the nth. The marked points do not coincide with the vertices of the n-gon. You can choose no more than one of the marked points from each side and form a convex non-degenerate polygon by connecting all those points with lines. Now your task is to find the number of different k-gons that can be formed that way.

</p><h3>Input</h3>
<p>The first line of input file contains positive integer t �C the amount of test cases. Next t lines contain six integers each: n, k, a, b, c, m. Here n is the number of sides of the initial n-gon. The amount of marked points on the first side of this n-gon is x<sub>1</sub> = a, the amount of the marked points on the following sides is x<sub>i</sub> = (b*x<sub>i-1</sub> + c) mod m, for i &gt; 1.

</p><h3>Constraints</h3>
<p>1 &lt;= t &lt;= 30<br>
3 &lt;= n &lt;= 10<sup>9</sup><br>
3 &lt;= k &lt;= 20<br>
1 &lt;= b, c, m &lt;= 10<sup>6</sup><br>
0 &lt;= a &lt; m

</p><h3>Output</h3>
<p>For each test case output the number of k-gons that can be formed modulo 1000000007.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
4 3 1 2 2 191
10 5 1 113 157 999991

<b>Output:</b>
1228
328836201


</pre>