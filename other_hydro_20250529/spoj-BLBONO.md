<p>Kang and Kung are board games enthusiast. However, they only like to play deterministic games, such as chess. Since there are only a few deterministic games, they decided to create a new one. This game is called 'Bono'.</p>
<p>The rule of Bono is simple. The board consist of a 3x3 grid. The game is turn based with 2 players. On each turn, the current player must fill an empty cell with a piece of water spinach. Players may not move any water spinaches that have been placed. The board will destroy itself if there is a row or column or diagonal consisting of 3 pieces of water spinach. A player loses if he can't make a move in his turn.</p>
<p>Of course, the first player will always win the game if he plays optimally. That is why they created Bono v2. In Bono v2, the number of boards used in a game is N (N<span style="text-decoration: underline;">&lt;</span>1000). On each turn, the current player must fill an empty cell on an undestroyed board with the same ruling as Bono. A player loses if he can't make a move in his turn.</p>
<p>Bono v2 is still too easy since if they both play optimally, player 1 will always win if N is odd, and player 2 will always win if N is even. To solve this matter, Bono v3 is created. In Bono v3, the initial state of each board might not be empty. Some cells might already be occupied with a piece of water spinach. Other than that, the rules are same as Bono v2.</p>
<p>Kang and Kung decide to play Bono v3 T times (T<span style="text-decoration: underline;">&lt;</span>1000). Kang always moves first and they both play optimally. For each game, who will win?</p>
<h3>Input</h3>
<p>First line of input is T, the number of games (T<span style="text-decoration: underline;">&lt;</span>1000).</p>
<p>For each game, first line is N, the number of boards (N<span style="text-decoration: underline;">&lt;</span>1000). Next N lines consists of the starting boards. A board is represented with a 9 digit binary string. Cell in (r, c) position is represented by (r-1)x3+c th character in the string. 0 means the cell is empty, 1 means the cell is filled.</p>
<h3>Output</h3>
<p>For each game, output a line containing the winner's name.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>1<br>000000000<br>2<br>000000000<br>000000000<br>2<br>100010000<br>001010000</pre>
<pre><strong>Output:</strong>
Kang<br>Kung<br>Kung&nbsp;</pre>