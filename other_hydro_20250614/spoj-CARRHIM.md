<p>Carrom board is a very popular game. There are four player in this game in dual player mode. In dual player game the team is pair with opposite side player.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img title="carrom" src="file://nIStqjrB.png" alt="carrom" width="600" height="600"></p>
<p>&nbsp;</p>
<p>So, in picture you see the board and the player��s.&nbsp; Where the player A and the player C in team-1, the player B and the player D in team-2.</p>
<p>In this game a team is play with one color pawn. So, if team-1 start playing the board they take the white pawn, and the team-2 get the black pawn for the game. If team-1 can cover all the pawn before the team-2 and the red also covered by the time then the team-1 will win. Otherwise team-2 will win if they cover their all pawn in the game.</p>
<p>Now, There are 9 white pawn and 9 black pawn and one red pawn in the board. The game is played by different rule.</p>
<p>In my problem of this game the rule like,</p>
<p>The point for the one pawn is 1 and for red is 5.</p>
<p>You can assume that which player 1st start playing&nbsp; the game is start with the white pawn.one team must cover red pawn and this team will get the red point.And you know the penalty rule is If one player cover one pawn of opposite team then the turn goes to the next player.</p>
<p>Now your task is to find the winner team &amp; points.</p>
<p>The points count by the remaining of pawn in the board and plus the covered red pawn point by the winning team.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><span style="font-size: medium;"><strong>Input<br></strong></span></p>
<p>Input consists of pairs of lines (at most 100 lines). Each pair contains 1 charecter and 3 integer.A first charecter is the player id(A , B , C or D) and three integer is W, B, R (1&lt;= W, B&lt;=9) separated by a space that is number of white, black and red pawn the player cover in his turn.The end of one input occurs when the first sequence starts with an "#" character (without the quotes).</p>
<p>&nbsp;</p>
<p style="text-align: center;"><span style="font-size: medium;"><strong>Output</strong><br></span></p>
<p>For each case if the game complete then you have to print a string ��Team-1 win and the point is N.�� (without the quotes) when team-1 win , Otherwise&nbsp;&nbsp; ��Team-2 win and the point is N.�� (without the quotes).</p>
<p>If the game is incomplete then print a string "Incomplete game." (without the quotes) when a team can not cover all the pawn of his turn.</p>
<p>N is the total point of winner team. See the sample input/output for exact formatting.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><span style="font-size: medium;"><strong>Sample</strong></span></p>
<p><strong> <span style="font-size: small;">Input :</span></strong></p>
<p>A 5 1 0</p>
<p>B 1 2 0</p>
<p>C 2 1 1</p>
<p>D 1 0 0</p>
<p>#</p>
<p>B 1 1 0</p>
<p>C 1 2 0</p>
<p>D 3 1 1</p>
<p>A 1 2 0</p>
<p>B 3 0 0</p>
<p>#</p>
<p>A 1 1 0</p>
<p>B 1 5 1</p>
<p>C 1 1 0</p>
<p>#</p>
<p><span style="font-size: small;"><strong>Output :</strong></span></p>
<p>Team-1 win and the point is 10.</p>
<p>Team-2 win and the point is 8.</p>
<p>Incomplete game.</p>
<p>&nbsp;</p>
<p><span style="font-size: small;"><strong>Explanation :</strong></span><br><br>For the first input player A start the game so the team-1 play with the white pawn.<br>After all input the team-1 cover all of white pawn also the red pawn.<br>and there are 5 black pawn remain in the board.<br>so, team-1 win and the point is 5+5=10.</p>
<p>____________________________________________________________________________________________________________</p>
<p><span style="white-space: normal;">&nbsp;</span><strong><span style="font-size: small;"><span style="font-family: 'comic sans ms', sans-serif;"><span style="text-decoration: underline;">Problem setter</span>: Md. Hashibul Amin Hemel, Dept. of CSE</span></span></strong><span style="white-space: normal;"> </span></p>
<p><strong><em><span style="font-size: small;"><span style="font-family: 'comic sans ms', sans-serif;">Bangladesh University of Business and Technology (BUBT)</span></span></em></strong></p>
<p><strong><span style="font-size: small;"><span style="font-family: 'comic sans ms', sans-serif;">&nbsp;</span></span></strong><span style="white-space: normal;"> </span></p>
<pre><span style="white-space: normal;"><pre><span style="white-space: normal;">
</span></pre>
</span></pre>
<p>&nbsp;</p>
<p>&nbsp;</p>