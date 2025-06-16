<p>Bahl and Debnath are always looking up for new exciting games on the internet. Yesterday, Bahl stumbled across a new game known as ¡°Totient Game¡±. He immediately showed that to Debnath. They found it pretty exciting and decided to play it. The game is as follows:</p>
<ol>
<li>The game is played with N piles of stones.</li>
<li>2 players play alternatively and at each turn a player selects a pile and divides it into two unequal sized piles ¡°i¡± and ¡°j¡± such that Totient(i)*Totient(j)=Totient(i*j) and i+j = no. of stones in that pile.</li>
<li>The player who is unable to make a move loses the game.</li>
</ol>
<p>Bahl insists on starting the game first. Can you predict the winner of the game? <strong>Assume that both player plays optimally.</strong></p>
<p><a href="http://en.wikipedia.org/wiki/Euler%27s_totient_function">http://en.wikipedia.org/wiki/Euler%27s_totient_function</a></p>
<h3>Input</h3>
<p>First line gives T, the number of test cases.</p>
<p>Each test starts with a line containing ¡°N¡±, the number of piles.</p>
<p>Next line gives N space separated integers. The i<sup>th </sup>integer represents the number of stones in the i<sup>th </sup>pile.</p>
<h3>Output</h3>
<p>Output T lines each containing the winner of the T games. Output ¡°Bahl¡± if Bahl wins the game or ¡°Debnath¡± if Debnath wins the game.</p>
<h3>Constraints</h3>
<p>1&lt;=T&lt;=10<br> 1&lt;=N&lt;=10^5<br> 1&lt;= No. of stones in each pile &lt;=10^7</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>1</pre>
<pre>3</pre>
<pre>1 2 3


<strong>Output:</strong>
Bahl</pre>