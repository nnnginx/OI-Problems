<p>Aman and Arpit are bored of coding. There is no challenge in it anymore, they feel. Bear in mind that even the problems which would appear very difficult for most of you are trivial for them. With ICPC approaching, their teammate, Sameer, is worried by this development. So, to rekindle their interest in coding, he challenges them to a game.</p>
<p>The game consists of an N*M grid (N rows, M columns). Some of the cells in the grid are occupied by coins. You can assume that all coins are identical. Sameer then gives them another grid of the same size, with a possibly different arrangement of coins. The objective is simple: the initial grid has to be transformed into the final grid, by moving coins. The following rules apply for coin movements:</p>
<ol>
<li>In one move, exactly one coin can be moved.</li>
<li>A coin can move one cell up, down, left or right in one move, provided that the destination cell is empty.</li>
<li>If the destination cell is occupied by another coin, then the current coin can jump over that particular coin to land in an empty cell. In fact, a coin can jump over any number of consecutive coins until it lands in an empty cell. It cannot jump over an empty cell. Irrespective of the number of coins it jumps over, it is still counted as one move.</li>
</ol>
<p>Whoever solves this in minimum number of moves will be the winner and will get a treat from Sameer. Since both Aman and Arpit really want to win, they immediately proceed to write code for the same. Can you help them predict the minimum number of moves in which the initial grid can be transformed into the final one?</p>
<h3>Input</h3>
<p>First line of input containts T, the number of test cases.</p>
<p>First line of each test case contains 2 integers, N and M, separated by a single space.</p>
<p>This is followed by 2*N lines per test case. The first N lines represent the initial grid and the next N lines represent the final grid.</p>
<p>Each character in the grid is either a ¡®C¡¯ or a ¡®.¡¯</p>
<p>&nbsp;¡®C¡¯ means that there is a coin on that cell, and ¡®.¡¯ means that the cell is empty.</p>
<h3>Output</h3>
<p>For each test case, output a single line containing the minimum number of moves required. If it is not possible to transform the original grid into the final one, output ¡®-1¡¯ (without quotes)</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>2</p><p>1 5</p><p>.CC..</p><p>CC...</p><p>3 3</p><p>C.C</p><p>.C.</p><p>C.C</p><p>...</p><p>CCC</p><p>.CC</p><strong>Output:</strong>
1</pre>
<pre>3</pre>
<pre><p>Explanation: In the first test case, the coin to the right can jump over the coin to the left in 1 move.</p></pre>
<pre><p><strong><br></strong></p><p><strong>Constraints:</strong></p><p><strong>1&lt;=T&lt;=10</strong></p><p>1 &lt;= N*M &lt;= 20</p></pre>