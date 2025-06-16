<p>Adrita loves to play with marbles at home. She has a circular table on her living room. Let it be sticked on the ground and the ground be a 2D space having only 2 coordinates x and y. She knows the equation of the circle to be x^2 + y^2 - px - qy + z = 0</p>
<p>She has N number of marbles of radius 1 unit. The table is not polished and Adrita has some coordinates where she wants to put the marbles.</p>
<p>Help her calculating the number of marbles she will place on the table. Consider the thickness of the table is negligible and if the center is on the border of the table the marble is considered to be on the table.</p>
<h3>Input</h3>
<p>The first line contains an integer T (1 &lt;= T &lt;= 10) denoting number of test cases and then T set of input follows of which. the first line contains values of p, q, z (1 &lt;= p, q, z &lt;= 10^6) of the equation x^2 + y^2 - px - qy + z = 0 and the next line contains an integer N (1 &lt;= N &lt;= 10^6) denoting the number of marbles Adrita has and then another N lines follows containing x, y ( -10^5 &lt;= x, y &lt;= 10^5) denoting the coordinates of the marbles.</p>
<h3>Output</h3>
<p>Print the number of marbles on the table.</p>
<h3>Example</h3>
<h4>Input</h4>
<pre>1
100 250 8125
5
30 10
-100 100
20 5
100 100
-30 10</pre>
<h4>Output</h4>
<pre>1</pre>