<p>One day Ohani and her friend was playing a game. The rules of the game is given below:</p>
<ol>
<li>Ohani Starts the game. Then the&nbsp; two player take turns.</li>
<li>At the starting of the game, Ohani and her friend together choose a number N.</li>
<li>They take the absolute value of N , N = |N| or, N = abs(N).</li>
<li>In one turn: a player chooses a divisor X of N where 1 &lt; X &lt;= N. Then he/she divides N by X. Then next player continues to do step 4 until N is not equal to 1.</li>
<li>The game ends when N becomes 1.</li>
<li>The player who can¡¯t make his/her next move, looses the game. Both the player plays optimally.</li>
</ol>
<p>Ohani and her friend was playing the game for a long time. So, they got bored. Then suddenly one interesting idea came to Ohani¡¯s mind. She wants to choose maximum number of ways to get 1 from N such that no two way has a common number except 1 and N?</p>
<p>For explanation:</p>
<p>Suppose N = 20.</p>
<p>Two possible way to get 1 is: 20-&gt;10-&gt;5-&gt;1&nbsp;&nbsp; and 20-&gt;5-&gt;1, both the way has number 5 in common.</p>
<p>But: 20-&gt;10-&gt;1 and 20-&gt;4-&gt;2-&gt;1 has no number common without 20 and 1.</p>
<p>So, now Ohani wants to know the number of ways such that no two way has common number except 1 and N. But Ohani is very weak in coding. So, she wants you to help.</p>
<h3>Input</h3>
<p>The first line of the input contains the number of testcases T ( &lt;= 100000).</p>
<p>Each of the next T lines contains a number N ( |N| &lt;= 1000000 ).</p>
<h3>Output</h3>
<p>For each testcase, output the desired answer. If it is impossible to reach 1, just print ¡°Impossible¡±.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>3<br>1<br>2<br>3&nbsp;</p>
<strong>Output:</strong>
0<br>1<br>1&nbsp;</pre>