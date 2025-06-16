<p>Charlesbert and Merangelou are playing a two-player game on a game board. The game board consists of several circles, where some circles are connected to other circles. Charlesbert uses a game piece called the GoalPiece, and Merangelou uses a game piece called the ChasePiece.
<br><br>
The game is played as follows: at the start of the game, Charlesbert chooses a circle on the board and places the Goalpiece on it, and at the same time Merangelou places the ChasePiece on circle 1. During the next K seconds, Merangelou makes a sequence of moves (at one move per second), where a move consists of either leaving the ChasePiece on its current circle, or moving the ChasePiece from its current circle to a circle that is directly connected to it. If the ChasePiece and the GoalPiece lie on the same circle before or exactly K seconds after Charlesbert last placed the ChasePiece, Merangelou wins. Otherwise, Charlesbert chooses a new circle on the board and places the GoalPiece on it, and Merangelou will make K more moves (Charlesbert moves the GoalPiece before Merangelou makes another move). This process is repeated until the ChasePiece and the GoalPiece lie on the same circle. Note that it is possible for Merangelou to win in fewer than K moves.
<br><br>
Merangelou wants to win the game as quickly as possible, while Charlesbert wants to keep the game going for as long as possible. Assuming both players play optimally, find the shortest amount of time (in seconds) after which Merangelou is guaranteed to have won the game. If Merangelou cannot win the game (i.e. if Charlesbert can keep the game going forever), then print "INFINITE GAME" instead.


</p><h3>Input</h3>
<p>The first line of the input contains a positive integer C (0&lt;C&lt;100), the number of test cases to follow. Each case begins with a line containing a two positive integers M and K (1&lt;M&lt;100, 0&lt;K&lt;100), representing the number of circles on the game board and the number of seconds between times that Charlesbert moves the ChasePiece. Each of the following M lines is a string of 'Y' and 'N' characters, with M characters per line. If the jth character of the ith line is 'Y', then circles i and j are connected, otherwise circles i and j are not connected. The jth character of line i will always be the same as the ith character of the jth line, and the kth character of the kth line will always be 'N'.  In other words, these M lines form an adjacency matrix for the circles. The ChasePiece always starts on the first circle.

</p><h3>Output</h3>
<p>For each case, if Merangelou can win then print the shortest amount of time required for her to win. Otherwise, print "INFINITE GAME". The output for each case should appear on its own line.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
5 1
NNNNY
NNNNY
NNNNY
NNNNY
YYYYN
4 2
NYNN
YNYN
NYNY
NNYN
4 1
NYNY
YNYN
NYNY
YNYN


<b>Output:</b>
2
4
INFINITE GAME

</pre>