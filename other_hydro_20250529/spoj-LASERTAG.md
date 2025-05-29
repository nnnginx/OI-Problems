<p style="text-align: justify;">As is tradition, one afternoon of Výberko is without a contest. On that afternoon, some fun optional activity is usually planned for those extroverted enough to go out and do something. One time, it was laser tag!<br><br>The battles were fierce, and the legends stay with us to this very day. At one point, they say, there was a temporary blackout on the battleground and the lights went out.<br><br>Each participant, at this point already a seasoned veteran with immaculate aim, prepared for the power to jump back on, reigniting the fierce battle. It was incredibly important to achieve as many points once it did, as surely the blackout caused the score counters to be reset to 0.<br><br>As all legendary warriors think alike, they all came up with the same strategy:<br><br>1. Point your laser gun north, i.e. in the positive Y-axis direction. (All participants are from Výberko, so it is ordinary for them to think in these terms.)<br><br>2. Once the power comes back on, start turning in the direction of your dominant hand at a constant speed of 1 degree per second.<br><br>3. Whenever you face someone, shoot them instantly. (If there are multiple people standing in that direction, shoot them all.)<br><br>4. After 360 seconds, when everyone is facing north again, stop and assess the results. Brag about your score.<br><br>Player A gets 1 point for shooting player B, if at that time player B has not shot player A yet.<br><br>All the participants came back to Výberko bragging about how many points they scored.<br><br>Paulinka stayed in the computer lab bashing her head against the 10 point problem that everyone else solved in the morning. Their bragging is getting on her nerves.<br><br>To take them down a notch, she decided to find out how many points everyone *really* got.<br><br>Since Paulinka can't even solve a 10 point problem, she needs your help!</p>
<p style="text-align: justify;"><strong>Task</strong><br><br>Each player can be modeled as a point in a 2D plane.<br>The Y axis grows in the direction from south to north and the X axis grows from west to east.<br>At time 0, each player is pointing their laser gun in the positive Y direction. Then, they start turning, either clockwise (right-handed) or anticlockwise (left-handed), all at the same angular velocity.<br><br>For the purposes of the problem, both the players and the laser have zero width, and the laser can shoot through players.<br><br>Player A gets 1 point for shooting player B if and only if A shot B first (B didn't shoot A yet).<br><br>Calculate the score of each player after they complete one full rotation.<br><br><strong>Input</strong></p>
<p style="text-align: justify;">The first line contains an integer <strong>t </strong>(<strong>1 ≤ t ≤ 20</strong>) - the number of games. <strong>t </strong>descriptions of games follow.</p>
<p style="text-align: justify;">For each game the first line contains an integer <strong>n</strong> (<strong>2 ≤ n&nbsp;≤ 300000</strong>) - the number of players. Sum of <strong>n</strong> in a single file will not exceed <strong>300000</strong>.<br><br><strong>n</strong> lines follow, each describing one player in the form <strong>x y h</strong>, where <strong>-10<sup>9</sup> <strong>≤ </strong> x,y <strong>≤ </strong> 10<sup>9</sup></strong> are their coordinates, and <strong>h</strong> is the character L if they're left-handed or R if they're right-handed.<br><br>Since players are generally introverted, they have instinctively positioned themselves on different <strong>x</strong> and <strong>y</strong> coordinates: all <strong>x</strong> coordinates in the input are distinct, and all<strong> y</strong> coordinates in the input are distinct.<br><br><strong>Output</strong><br><br>For each game output <strong>n</strong> lines, the <strong>i</strong>-th of which contains a single integer: the score of player number <strong>i</strong>, in the same order as they appeared in the input.<br><br><strong>Example</strong></p>
<p style="text-align: justify;"><strong>Input:<br></strong></p>
<pre>2
3
0 0 L
-2 1 R
-1 -1 R
3
0 0 R
-2 1 R
-1 -1 R
</pre>
<p style="text-align: justify;"><strong>Output:</strong></p>
<pre>1
1
1
0
2
1
</pre>
<p style="text-align: justify;"><strong></strong><br><br>In the first game, Player 1 shoots player 2 long before player 2 shoots player 1 back. Similarly, player 2 gets a point for shooting player 3 and player 3 for player 1. So this particular game looks a bit like rock-paper-scissors.</p>
<p style="text-align: justify;">Being right-handed would not turn out well for the first player. Now player 1 loses to both opponents.</p>