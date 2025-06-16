<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MTRGAME/en/">English</a></td> 
<td width="50%"><a href="/problems/MTRGAME/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>Players P1 and P2 are playing a game. The game is played using a matrix M of integers, the size of which is given to be m x n. </p>
<p>In each turn, P1 selects a number i lying between 0 and m-1 (inclusive) while P2 selects a number j lying between 0 and n-1 (again inclusive). The fun part is that each of them remains unaware of what the other has chosen...</p>
<p> After the choices have been finalized, they reveal their numbers to each other. M[i][j] is the element of the matrix decided by the choices the players made. If M[i][j] is Negative, P1 pays P2 an amount equal to the absolute value of M[i][j]. However, if M[i][j] is Positive, then P2 pays P1 an amount equal to M[i][j].</p> <p>Given the Matrix M and the fact that both the players are infinitely intelligent, find out the average amount paid by P2 to P1 per turn in the game.</p> 
<p>Note: P1 plays to maximize the money he gets while P2 tries to minimize the money he has to pay. </p>

<h3>Input</h3>
<p>First line contains T, the number of test cases.</p> <p>For each test case the first line contains two integers m and n, denoting the size of the matrix. The next m lines contains n integers each denoting the elements of the matrix. </p>

<h3>Output</h3>
<p>The output should consist of T lines, each containing a real number with exactly 3 digits precision, denoting the average payoff which P1 receives per turn in the game. </p>

<h3>Example</h3>

<pre><b>Input:</b>
3
1 1
-1
2 2
1 2
3 4
2 2
1 4
4 3


<b>Output:</b>
-1.000
3.000
3.250
</pre>

<h3>Constraints</h3>
<p>
Input Set 1: m &lt;= 2, n &lt;= 10, abs(values) &lt;= 150000, numberOfTestCases &lt;= 120.</p>
<p>Input Set 2: m &lt;= 2, n &lt;= 5000, abs(values) &lt;= 150000, numberOfTestCases &lt;= 20.</p> 
<p>Input Set 3: m &lt;= 2, n &lt;= 100000, abs(values) &lt;= 150000, numberOfTestCases &lt;= 10.</p>
<p>Input Set 4: m &lt;= 3, n &lt;= 5000, abs(values) &lt;= 150000, numberOfTestCases &lt;= 15.</p>