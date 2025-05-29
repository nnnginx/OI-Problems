<p>Tom and Hanks play the following game. On a game board having a line of squares labelled from 0,1,2 ... certain number of coins are placed with possibly more than one coin on a single square. In each turn a player can move exactly one coin to any square to the left i.e, if a player wishes to remove a coin from square i, he can then place it in any square which belongs to the set (0,1, ... i-1) . The game ends when all coins are on square 0 and player that makes the last move wins. Given the description of the squares and also assuming that Tom always makes the first move you have tell who wins the game (Assuming Both play Optimally).</p>
<h3>Input</h3>
<p>The first line will contain N the number of test cases and then 2N lines follow. For each test case the first line will have S the size of the board and in the next line S integers follow. The i<sup>th</sup> integer gives the the number of coins in the i<sup><sub>th</sub></sup> square (starting from 1) . Atleast one of the S integers will be non zero. All the numbers in the input will be less than 25.</p>
<h3>Output</h3>
<p>For each test case output one line containing either "Tom Wins" or "Hanks Wins".</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>1<br>1<br>1<br>2<br><strong><br>Output:</strong>
<br>Tom Wins<br>Hanks Wins</pre>