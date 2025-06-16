<p style="margin-bottom: 0.14in; line-height: 115%;">Amit is a big fan of Nim Game. Literally! He doesn¡¯t just play the game, he fantasizes it. He follows the simple mantra ¨C Eat, Sleep, Nim. His fantasy is overgrown over time that he has starting thinking of himself as God of Nim. Legend has that if you meet him, more often than not he is imagining a game played between you both and how he beats you with comfort.</p>
<p style="margin-bottom: 0.14in; line-height: 115%;">Frustrated with his never ending Nim fantasy, Mishra decides to give him a taste of his own medicine. Mishra devises a game which looks similar to Nim but is not in reality. Here¡¯s how the game looks:</p>
<ol>
<li>
<p style="margin-bottom: 0.14in; line-height: 115%;">Game is 	played between 2 players, taking turns alternatively. Both play 	optimally.</p>
</li>
<li>
<p style="margin-bottom: 0.14in; line-height: 115%;">There are N 	plies of coins, each containing exactly Pi coins.</p>
</li>
<li>
<p style="margin-bottom: 0.14in; line-height: 115%;">There are N 	integers given. Let¡¯s denote each of them by Ki.</p>
</li>
<li>
<p style="margin-bottom: 0.14in; line-height: 115%;">In a single 	turn, a player can choose a pile Pi and can discard ¡°x¡± coins 	from the pile Pi where 1&lt;=x&lt;=Ki. For example ¨C if pile P1 is 	chosen by a player, then he can discard x coins such that 1&lt;=x&lt;=K1.</p>
</li>
<li>
<p style="margin-bottom: 0.14in; line-height: 115%;">Amit always 	starts the game. The player who cannot make a move loses the game.</p>
</li>
</ol>
<p style="margin-bottom: 0.14in; line-height: 115%;">If Mishra beats Amit in this game, Amit will have no option but to shed his Nim ego and so we all will be saved. Can you find out if Mishra succeeds?</p>
<h3>Input</h3>
<p style="margin-bottom: 0.14in; line-height: 115%;">First line contains T, the number of test cases. Each test cases starts with an integer N in first line. Next line consists of N integers, P1 to PN. Next line consists of N integers, K1 to KN.</p>
<p style="margin-bottom: 0.14in; line-height: 115%;">1&lt;=T&lt;=10</p>
<p style="margin-bottom: 0.14in; line-height: 115%;">1&lt;=N&lt;=10000</p>
<p style="margin-bottom: 0.14in; line-height: 115%;">0&lt;=Pi&lt;=10^9</p>
<p style="margin-bottom: 0.14in; line-height: 115%;">1&lt;=Ki&lt;=10^9</p>
<h3>Output</h3>
<p style="margin-bottom: 0.14in; line-height: 115%;">Output exactly one string per test case, ¡°Mishra¡± if Mishra wins the game or ¡°Amit¡± if Amit wins the game.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p style="margin-bottom: 0.14in; line-height: 115%;">2</p><p style="margin-bottom: 0.14in; line-height: 115%;">1</p><p style="margin-bottom: 0.14in; line-height: 115%;">5</p><p style="margin-bottom: 0.14in; line-height: 115%;">2</p><p style="margin-bottom: 0.14in; line-height: 115%;">2</p><p style="margin-bottom: 0.14in; line-height: 115%;">4 7</p><p style="margin-bottom: 0.14in; line-height: 115%;">1 3</p>

<strong>Output:</strong>
<p style="margin-bottom: 0.14in; line-height: 115%;">Amit</p><p style="margin-bottom: 0.14in; line-height: 115%;">Amit</p><p style="margin-bottom: 0.14in; line-height: 115%;">&nbsp;</p><p style="margin-bottom: 0.14in; line-height: 115%;">Explanation:</p><p style="margin-bottom: 0.14in; line-height: 115%;"><span style="line-height: 115%;">For second test case, one possible way of winning for Amit is ¨C Amit and Mishra discard 1 coin alternatively from first pile, starting from Amit. Then Amit picks up 3 from second pile, Mishra picks up 1 from second pile and Amit finishes the game by picking up 3 coins left in the second pile.</span></p></pre>