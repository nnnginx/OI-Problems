<p>Ada the Ladybug was recently unwrapping presents and guess what? She got a new chessboard from her good friend Flea Feodorv. As he though "the bigger chessboard the better the chess game will be", he gave Ada a chessboard even bigger than last time: Now the upper-right corner is [999999999,999999999] (10<sup>9</sup>-1).</p>
<p>As you might guess, she can't play classical (nor rapid) chess on such board. But as she doesn't to throw such valuable (well.. at least big) gift away, she've decided to play <a href="../../ADAGAME5/">Palace Game</a> again. She invited her friend Velvet Mite Vinit. As they played this game recently, they decided to expand the rules a little bit. They have decided to play this game with five most important chess-pieces: <strong>Rook</strong>, <strong>Bishop</strong>, <strong>King</strong>, <strong>Knight</strong> and obviously, the <strong>Palace</strong>.</p>
<p>The game rules are simple: A few <strong>chess-pieces</strong> are placed onto chessboard. Ada and Vinit alternate in moves. In each move one can choose any <strong>piece</strong> on chessboard and move it toward bottom-left corner. Moving toward means, that the <a href="https://en.wiktionary.org/wiki/Manhattan_distance">Manhattan     distance</a> from bottom-left corner will decrease and also that none of the coordinates of chess-piece will increase. A player who can't make a move will lose. Can you tell who'll be the winner if both of them play optimally? As Ada is a lady, she goes first.</p>
<p>NOTE: Rules are <em>slightly</em> different than in original Palace Game (even though it wouldn't affect the original game, this game might yield slightly different results).</p>
<h3>Input</h3>
<p>The first line of input will contain <strong>1 ¡Ü T ¡Ü 3*10<sup>5</sup></strong>, the number of test-cases.</p>
<p>&nbsp;</p>
<p>The next <strong>T</strong> lines will contain <strong>1 ¡Ü N ¡Ü 3*10<sup>5</sup></strong>, the number of chess pieces placed on chessboard.</p>
<p>&nbsp;</p>
<p>Each test-case will contain <strong>N</strong> lines containing two integers and a character: <strong>0     ¡Ü x, y &lt; 10<sup>9</sup></strong>, the coordinates of chess-piece and <strong>c ¡Ê</strong> {T, B, K, N, P} (stands for rook(<strong>T</strong>), <strong>B</strong>ishop, <strong>K</strong>ing, k<strong>N</strong>ight and <strong>P</strong>alace).</p>
<p>&nbsp;</p>
<p>The sum of <strong>N</strong> over all test-cases will not exceed <strong>3*10<sup>5</sup></strong></p>
<h3>Output</h3>
<p>For each test-case output the name of winner, so either "Ada" or "Vinit".</p>
<h3>Example Input</h3>
<pre>10
2
7 0 B
3 4 T
2
6 7 K
9 1 B
3
8 7 B
9 4 K
4 4 T
2
8 5 T
6 5 K
3
1 2 P
6 1 B
4 4 P
2
1 2 B
0 9 K
1
1 9 K
3
5 0 K
0 4 B
9 1 K
3
0 4 K
0 5 K
3 2 K
3
6 4 N
1 2 N
0 7 N
</pre>
<h3>Example Output</h3>
<pre>Ada
Vinit
Ada
Ada
Ada
Vinit
Ada
Ada
Vinit
Vinit
</pre>