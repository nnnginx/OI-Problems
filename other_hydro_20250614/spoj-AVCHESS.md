<p>The Avengers become divided, both over how to approach Loki and the  revelation that S.H.I.E.L.D. plans to harness the Tesseract to develop  weapons as a deterrent against hostile extraterrestrials. The argument  is raised between Captain America, Iron man and Thor each having his own  point to keep. Agent Natasha Romanoff comes up with a non-violent  solution to this argument by suggesting a variant of the game of chess  for three players. This time chessboard contains only a knight, a rook  and a bishop. In this game, first Captain America takes his turn, next  Iron Man and then Thor. After Thor's turn, this sequence repeats.</p>
<ul>
<li>Captain America can only move knight, Iron Man rook, and Thor bishop  and each player can move their respective piece to an empty position. </li>
<li>The rook can move any number of squares horizontally or vertically, but may not leap over other pieces. </li>
<li>The bishop can move any number of squares diagonally, but may not leap over other pieces.</li>
<li>The knight' move forms an "L"-shape: two squares vertically and one  square horizontally, or two squares horizontally and one square  vertically. The knight is the only piece that can leap over other  pieces.</li>
</ul>
<p><br> The objective of game is to place rook at the initial position of  knight, bishop at initial position of rook and knight at initial  position of bishop. That is, if the initial position of knight, rook and  bishop is <strong>(x1, y1), (x2, y2)</strong> and <strong>(x3, y3)</strong>, respectively, then the final position of them should be <strong>(x3, y3), (x1, y1), (x2, y2)</strong> respectively.</p>
<h3>Input</h3>
<p>The first line of the input contains an integer T denoting the number of test cases.<br> Each test case consists of exactly one line containing 6 space separated integers <strong>x1 y1 x2 y2 x3 y3</strong>.<br> <strong>x1 y1</strong> represents the initial position of Knight.<br> <strong> x2 y2</strong> represents the initial position of Rook.<br> <strong> x3 y3</strong> represents the initial position of Bishop.</p>
<ul>
<li><strong>T</strong>=<strong>5</strong></li>
<li><strong>0</strong> �� <strong>x1, y1</strong> �� <strong>7</strong></li>
<li><strong>0</strong> �� <strong>x2, y2</strong> �� <strong>7</strong></li>
<li><strong>0</strong> �� <strong>x3, y3</strong> �� <strong>7</strong></li>
<li>No pair of initial positions are equal, i.e., (<strong>x1</strong>, <strong>y1</strong>) != (<strong>x2</strong>,<strong> y2</strong>) &amp;&amp; (<strong>x1</strong>, <strong>y1</strong>) != (<strong>x3</strong>, <strong>y3</strong>) &amp;&amp; (<strong>x2</strong>, <strong>y2</strong>) != (<strong>x3</strong>, <strong>y3</strong>)</li>
</ul>
<h3>Output</h3>
<p>For each test case, print the minimum number of turns required to achieve this objective.</p>
<p>If the desired configuration is not reachable print -1.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
0 0 5 1 3 3 

<strong>Output:</strong> 
5
</pre>
<h3>Explanation</h3>
<p>Starting Points of Knight[0,0], Rook[5,1] and Bishop[3,3] can be changed to Knight[3,3], Rook[0,0], Bishop[5,1] in the following five steps:<br> Knight - [0,0] to [1,2]<br> Rook - [5,1] to [5,0]<br> Bishop - [3,3] to [5,1]<br> Knight - [1,2] to [3,3]<br> Rook - [5,0] to [0,0]</p>
<p>There is no way to get the required final configuration in less than 5 steps.</p>