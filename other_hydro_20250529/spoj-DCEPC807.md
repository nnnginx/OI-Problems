<p>Alice and Bob play an interesting game. They start with a number ¡°n¡± and follow some rules until the game ends. The rules for the game are:</p>
<ol>
<li>Let F(n) denotes the total no. of set bits in binary representation of numbers from 0 to (2^n) -1.</li>
<li>Each player plays alternatively until the game ends and one of them wins the game.</li>
<li>In each turn a player either unsets a single set bit from binary representation of ¡°n¡± or unsets 2 consecutive set bits from the binary representation of ¡°n¡±. Let¡¯s call the resulting number after such move as ¡°x¡±.</li>
<li>The game ends when F(x) is a power of 2. (0 is also a power of 2).</li>
<li>The player with no move loses the game and so other player wins the game.</li>
<li>Alice starts the game always.</li>
<li>Both of them play optimally.</li>
</ol>
<p>Given ¡°n¡± can you predict the winner of the game?</p>
<h3>Input</h3>
<p>First line contains T, the no. of test cases.</p>
<p>Next T lines contains one integer per line, ¡°n¡± (quotes for clarity).</p>
<h3>Output</h3>
<p>Output T lines, each containing either ¡°Alice¡± if Alice wins the game or ¡°Bob¡± if Bob wins the game.&nbsp;</p>
<h3>Constraints</h3>
<p>1&lt;=T&lt;=10</p>
<p>0&lt;=N&lt;=10^6</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>4</pre>
<pre>10</pre>
<pre><strong>Output:</strong>
Bob</pre>
<pre>Alice</pre>