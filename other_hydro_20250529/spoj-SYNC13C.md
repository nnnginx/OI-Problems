<p>Ramesh and Suresh get a box full of five stars on lottery each. Since both the boxes need not have the same number of chocolates, they decide to play a game. The winner gets to have both the boxes of chocolates. They play alternatively and Suresh starts the game.</p>

<p>Given the number of chocolates in both the boxes, let them be c1 and c2, the player takes either c1 or c2 number of chocolates and divide the remaining box of chocolates to two boxes (these two boxes need not have the same number of chocolates). The player who cannot make such a move loses.</p>

<p>Given the initial number of chocolates (c1 and c2) find the winner.Assume both the players play optimally.</p>

<h3>Input</h3>
<p>First line of input contains a number T (1 &lt;= T &lt;= 1000), the number of test cases. Then follows T lines each containing two space separated integers c1 and c2</p>
<p>(1 &lt;= c1 &lt;= c2 &lt;= 10000).</p>

<h3>Output</h3>
<p>For each test case print "<code>Ramesh</code>" or "<code>Suresh</code>" depending on who is the winner.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 1
4 5

<strong>Output:</strong>
Ramesh
Suresh</pre>