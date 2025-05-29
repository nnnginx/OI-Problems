<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Manoj and Pankaj play the following game on a N*M grid, Each cell of which is either empty or contain a stone.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each player in his his turn must take one the two moves described below:-</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1. He can shift an stone to its adjacent right cell, if that cell is empty</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2. or he can remove a stone completely from the grid.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Player who take the last turn will wins the game. It is also given that both the players will play optimally and Manoj always take the first turn.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">You have to find who will win the game.&nbsp;</div>
<p>Manoj and Pankaj play the following game on a N*M grid, Each cell of which is either empty or contain a stone.</p>
<p>Each player in his his turn must take one the two moves described below:-</p>
<p>1. He can shift an stone to its adjacent right cell, if that cell is empty</p>
<p>2. He can remove a stone completely from the grid.</p>
<p>1st player who is unable to take a move looses the game . It is also given that both the players will play optimally and Manoj always take the first turn.</p>
<p>You have to find who will win the game.&nbsp;</p>
<h3>Input</h3>
<p>First line of each test case contains two integers N and M. (1&lt;=N,M&lt;=200) Each of next&nbsp;N lines contains an string, jth character on of ith string is '*' if there is an stone otherise it is '.' (empty). Input ends when N, M = 0,0. which is not to be processed.</p>
<h3>Output</h3>
<p>For each test case print 'Manoj' if Manoj wins, print 'Pankaj' otherwise.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>

2 2
.*
.*

2 2
.*
*.
0 0</pre>
<pre><strong>Output:</strong>
Pankaj
Manoj</pre>