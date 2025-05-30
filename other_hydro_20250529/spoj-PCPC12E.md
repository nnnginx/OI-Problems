<p><span style="font-size: small;">Snakes and Ladders (or Chutes and Ladders) is an ancient Indian board game regarded today as a worldwide classic. It is played between two or more players on a game board having numbered squares (fields) on a grid. A number of "ladders" and "snakes" (or "chutes") are pictured on the board, each connecting two specific board squares. The object of the game is to navigate one's game piece from the start (Bottom square) to the finish (Top Square), helped or hindered by ladders and snakes, respectively. The historic version had root in morality lessons, where a player's progression up the board represented a life journey complicated by virtues (ladders) and vices (snakes). &nbsp;If, after throwing a dice, a player's token lands on the lower-numbered end of a "ladder", the player moves his token up to the ladder's higher-numbered square. If he lands on the higher-numbered square of a "snake" (or chute), he must move his token down to the snake's lower-numbered square. If any of those cases takes places, we will call a square unstable. Otherwise it is stable.</span></p>
<p><span style="font-size: small;">The game is a simple race contest lacking a skill component, and is popular with young children.</span></p>
<p><span style="font-size: small;">In this problem you��re required to calculate the minimum number of 6-sided die throws to move your game piece from the start (bottom square) to the finish (top square).</span></p>

<br>
<p><span style="font-size: small;"><strong>Formal game description</strong></span></p>
<p><span style="font-size: small;">Fields are arranged on an NxM grid and numbered from 1 to N*M. Last field, indicated by N*M, is referred to as Top Square. Each player starts with a token on a square at position "0" (the imaginary space beside the ��1�� grid field; Bottom Square), which is always stable. So in total we have N*M+1 fields. In every turn player throws the die and moves up by the given number of squares. If that would result in a field higher than Top Square, then token is not moved. If the square that token ends on is unstable, it is moved as indicated by ladder or snake. This is repeated until token is placed a stable field. You can assume that a stable field can be reached from any field on the board. If this final, stable field is the Top Square, game ends and player wins.</span></p>

<br>
<p><span style="font-size: small;">&nbsp;<img title="PIC" src="/content/zukow:snakes_and_ladders.png" alt="PIC" width="341" height="259"></span></p>

<br>
<p><span style="font-size: small;"><strong>Input Specification</strong></span></p>
<p><span style="font-size: small;">Input contains multiple test cases First line of each test case contains integers N, M, S, L. where n and m are the board dimensions, N (0 &lt; N &lt;= 100), M (0 &lt; M &lt;= 100), and S and L are number of snakes and ladders respectively. Next S lines describes snakes. Each line contains two integers: h and t, where h is the snake��s head position and t is the snake tail position. (0 &lt; t &lt; h &lt;=N*M), Next L lines describes ladders. Each line contains two integers: p and q where p is the ladder��s bottom and q is the ladder��s top (0 &lt; p &lt; q &lt; N*M).</span></p>
<p><span style="font-size: small;">The input will be terminated by the end of file.</span></p>

<p><b><span style="font-size: small;">NOTE! There could be more snakes and/or ladders leading from a single field. In such a case use the last snake/ladder specified in the input.</span></b></p>

<br>
<p><span style="font-size: small;"><strong>Output Specification</strong></span></p>
<p><span style="font-size: small;">Print one line per test case containing the minimum number of dice throws. If you cannot reach to the finish square print -1</span></p>

<br>
<pre><strong>Sample Input</strong>

1 1 0 0
1 2 1 0
2 1
5 10 3 5
16 6
47 26
49 11
1 38
4 14
9 31
40 42
36 44
</pre>

<br>
<pre><strong>Sample Output</strong>

1
-1
3
</pre>
<br>

<p><strong style="color: #000020; font-size: 13px; text-align: justify; background-color: #f6f9e0;">See also:&nbsp;</strong><a href="../PCPC12F/"><span style="font-size: medium;">Snakes and Ladders Again</span></a></p>