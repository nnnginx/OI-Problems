<p>&nbsp;</p>
<p>Dixon was in his house, he was a little bored, so he took some dominoes from the case and started thinking: ��It is possible to use Qx pieces from the Dominoes so it can make a simulation of a game?�� so, Dixon is not a super programmer, but he knows a little bit of constraints in the problems, so he will give it to you, your task, if you choose to accept it, is to find all the possible ways of some N pieces of Domino can be joined together to make a game simulation using exactly Qx dominoes pieces. If you can��t do this, you should print ��0��</p>
<p><img title="Dominoes" src="../../../../../../content/simes:DIXDOOM.jpg" alt="Dominoes"></p>
<p>INPUT:</p>
<p>The input will consists of an integer T, denoting the number of test cases, next, T cases will follow, every case starts with 2 lines N and Q, being N the number of dominoes David has and Q the number of queries you should do, then, N lines will follow, denoting the two parts of a domino piece, as you may know, the domino piece is split in two, so you can join by any side another piece, after this, Q lines will follow, denoting the number of piece you must use to build the game simulation.</p>
<p>&nbsp;</p>
<p><strong>CONSTRAINTS:</strong></p>
<p>1&lt;=T&lt;=100</p>
<p>1&lt;=N&lt;=16</p>
<p>1&lt;=Q&lt;=16</p>
<p>0&lt;=N<span style="font-size: xx-small;"><span style="font-family: arial, helvetica, sans-serif;">1</span></span>,��,N<span style="font-size: xx-small;"><span style="font-family: arial, helvetica, sans-serif;">N</span></span>&lt;=6</p>
<p>1&lt;=Q<span style="font-size: xx-small;"><span style="font-family: arial, helvetica, sans-serif;">1</span></span>,��,Q<span style="font-size: xx-small;"><span style="font-family: arial, helvetica, sans-serif;">N</span></span>&lt;=N</p>
<p>&nbsp;</p>
<p><strong>OUTPUT:</strong></p>
<p>You should output <strong>all</strong> the possible ways to form a game using Qx pieces (with any possible permutation too), as this number can grow very huge, we need you to print the output modulo 31337.</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>3<br>4 3<br>2 3<br>3 1<br>1 4<br>4 3<br>1<br>3<br>4<br>2 1<br>1 2<br>1 2<br>2<br>2 1<br>1 1<br>1 1<br>2</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>8</p>
<p>10</p>
<p>4</p>
<p>4</p>
<p>8</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>Domino idea credits goes to: <a href="../../users/danielmaxx/">Daniel Ampuero</a> and <a href="../../users/el_primo/">Luis Arguello</a></p>
<p>&nbsp;</p>
<p>Example of the output with the first case and Q=4</p>
<p>solution 1: joining the pieces 1,2,3 and 4</p>
<p>solution 2: joining the pieces 4,3,2 and 1</p>
<p>solution 3: joining the pieces 2,3,4 and 1</p>
<p>solution 4: joining the pieces 1,4,3 and 2</p>
<p>&nbsp;</p>
<p><strong>Tip: </strong>In the case with one piece only, you can form a game starting with the two faces of every single piece, i.e. if we want to form a game using just the piece "2 1", one possible game is "2 1" and the other "1 2", resulting in two different ways.</p>