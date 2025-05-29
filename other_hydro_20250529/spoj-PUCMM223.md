<p>You and Me is a board game between two players, the board is MxN, with 1 ¡Ü M,N ¡Ü 20. Initially each player has one piece, piece 'a' and piece 'b', both players move at the same time its piece, a valid move is to move the piece one square on each of the 4 cardinal directions (North, South, East, West),or stay in the same square, that is, if a piece is at x,y it can move to(x-1, y), (x, y-1), (x, y), (x, y+1), (x+1, y), so with the two pieces combined there are 5x5=25 possibilities in one move. The game has a goal, piece 'a' must finish at position initially accupied by 'b', and viceversa. To make this game more interesting the cells can be occupied by a block('#'), or can be unocuppied('.'). What is the minimum number of moves required to achieve this goal, if the pieces cannot occupy the same square at a given time and can't cross each other. See examples for further details.</p>
<h3>Input</h3>
<p>For each test case the first line contains two separated integers, M and N, rows and columns of the board.</p>
<p>then M strings of N characters follow.</p>
<p>Each character could be '.', '#', 'a', 'b'.</p>
<p>Just one 'a' and one 'b' exists.</p>
<p>The last case is followed by 0 0.</p>
<h3>Output</h3>
<p>Output the minimum number of moves required to achieve the goal. Output IMPOSSIBLE if it is not possible.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3 4<br>#..#<br>a..b<br>####<br>3 7<br>#######<br>#a...b#<br>#######<br>4 4<br>a...<br>###.<br>##..<br>b...<strong><br>0 0<br>Output:</strong><br>5<br>IMPOSSIBLE<br>11<br><br>Note:<br>1st case:<br>one possibility is<br>#..#    #..#    #.b#    #..#    #..#    #..#<br>a..b---&gt;.ab.---&gt;..a.---&gt;..ba---&gt;.b.a---&gt;b..a<br>####    ####    ####    ####    ####    ####<br></pre>