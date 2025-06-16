<p>Goran and Stjepan play an interesting game. On the table between them, there is a sequence of N skyscrapers made of Lego bricks. All of them are made of equal bricks and each of them has a height, which equals the number of bricks in it.</p>
<p>Goran plays first; then Stjepan, then Goran, then Stjepan and so on. In each move, a player has to find the <strong>highest</strong> skyscraper in the sequence (if there's more than one, he chooses any of them) and reduces its height - that is, takes away an arbitrary (positive) number of bricks from it.</p>
<p>The winner of the game is the one who takes away the last brick. Equivalently, the loser of the game is the one who is not able to make a move.</p>
<p>Help Goran and tell him in how many ways he can play his first move, so that he can certainly win (no matter how Stjepan played). If Goran doesn't have a winning strategy at all, the number of ways is zero.</p>
<h3>Input</h3>
<p>In the first line of input, there is an integer T ¡Ü 3, the number of test cases.</p>
<p>Then follow T blocks, each of them in two lines:</p>
<p>- N ¡Ü 300 000, the number of skyscrapers in the sequence</p>
<p>- a sequence of N integers in the range [0, 10<sup>6</sup>]</p>
<h3>Output</h3>
<p>For each of the T games, print the required number of ways.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>3</p><p>5</p><p>0 1 0 1 0</p><p>3</p><p>0 7 0</p><p>5</p><p>1 0 1 0 1</p>
<strong>Output:</strong>
0</pre>
<pre>1</pre>
<pre>3</pre>