<p>Pranjali and Nancy are playing an amazing game. The game starts with a string of bits (i.e. string of 0¡¯s and 1¡¯s). Game progresses in the form of right to left bit by bit scans. Pranjali takes turn when a ¡°1¡± bit comes while scanning the string and Nancy takes turn when a ¡°0¡± bit comes while scanning. In their respective turns, they can either choose to toggle their bit or keep it unchanged. The goal is to make all bits 0 at the end of scan, failing which means the scanning starts again from right to left. If all the bits are 0 at the end of a scan, the game ends and Pranjali is declared a winner. There is no win for Nancy. The game either ends to the goal described or the scanning continues indefinitely. So it can be seen that Pranjali has to win the game and in an optimal number of scans whereas Nancy¡¯s aim is to not let Pranjali win (by making it an indefinite play) or to delay Pranjali¡¯s win if it¡¯s sure. So now assuming that they both play with their optimal strategy, can you please tell if Pranjali can win the game or not?</p>
<p>Note: There has to be AT LEAST 1 scan before the game can end.</p>
<h3>Input</h3>
<p>First line contains T, the number of test cases.</p>
<p>Each of the next T lines contains a string of 0¡¯s and 1¡¯s.</p>
<h3>Output</h3>
<p>For each string given in the input, output either ¡°WIN m¡±, without quotes, if Pranjali can force her win in ¡°m¡± scans in an optimal play, or output ¡°INFINITE PLAY¡± if the game cannot be reached to the above mentioned goal in an optimal play.</p>
<h3>Constraints</h3>
<p>1&lt;=T&lt;=20</p>
<p>1&lt;= Length of string &lt;=50</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2</pre>
<pre>1</pre>
<pre>10

<strong>Output:</strong>
WIN 1</pre>
<pre>WIN 2</pre>
<h3>Explanation</h3>
<p>In the 2<sup>nd</sup> test case, during the first scan, Nancy gets the first turn because the right most bit is 0. She has to toggle it or the game will be over in a single scan. In the next turn, Pranjali chooses to keep her bit unchanged. So after first scan, the string is now ¡°11¡±. In the next scan, Nancy has no turns. So Pranjali will toggle both 1 bit and thus end the game.</p>