<p>Mr. Bitmann, the coach of the national soccer team of Bitland, is a perfectionist. He taught  his players optimal tactics and improved their endurance and shape. So they qualified  for the soccer woldcup this year. Due to his perfectionism the coach attaches importance not only to the performance in the game but also before the game.  So he told the team captain in what formation the team should assemble before the national anthem is played.  Since each of the 11 team members has a unique number between 1 and 11  on his shirt, he can represent the formation as a permutation of  numbers.</p>
<p>Before the first game the coach told  the captain that the team    should  line up  in increasing order (picture (d)). But  some players forgot the ordering and the orientation of the formation like  in picture (a). Only player 1 has the right orientation.  The coach went nearly mad when he saw this desaster!  How could he solve the problem?</p>
<p style="text-align:center;"><img src="../../../content/sgog:wm06.png" alt="scenario example"></p>
<p>"Hmmm... I'll let my players dance!". A great idea!               He took his notebook and started to create a choreography which leads to    his expected formation. Due to the fact that no one of the  players took dancing lessons he    restricts his dance to one basic move:  One player or more players who stand side by side can turn 180 degrees  around the center of the move. Picture (b) contains an example: The  players</p>
<pre style="text-align:center;">-11 -10 -9 -2</pre>
<p align="justify">(we mark players which stand in the wrong direction with  a minus) can do one move to</p>
<pre style="text-align:center;">2 9 10 11</pre>
<p align="justify">As perfect as he is he calculated a dance with a minimum number of moves. It works perfectly and now he's planning to do dancing performances                      with teams with more than 11 members. So he needs your help to find optimal dancing moves...</p>
<h3>Input</h3>
<p>Each testcase starts with the number of team members n (0&lt;=n&lt; 2200). The next lines represent the formation at the beginning and the expected formation at the end of the choreography.</p>
<h3>Output</h3>
<p>For each testcase output m, the minimal number of moves which are necessary  to reach the expected formation. The next m+1 lines should  represent one possible scenario of moves.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
11
-5 -4 -3 -8 -7 -6 1 -11 -10 -9 -2
1 2 3 4 5 6 7 8 9 10 11
11
1 2 3 -4 -5 -6 -7 -8 -9 10 11
11 9 8 7 6 5 4 3 2 10 1
0

<strong>Output:</strong>
3 Steps
-5 -4 -3 -8 -7 -6 +1 -11 -10 -9 -2
-5 -4 -3 -8 -7 -6 +1 +2 +9 +10 +11
-5 -4 -3 -2 -1 +6 +7 +8 +9 +10 +11
+1 +2 +3 +4 +5 +6 +7 +8 +9 +10 +11
5 Steps
+1 +2 +3 -4 -5 -6 -7 -8 -9 +10 +11
+1 +2 -3 -4 -5 -6 -7 -8 -9 +10 +11
+1 -2 -3 -4 -5 -6 -7 -8 -9 +10 +11
+1 -2 -3 -4 -5 -6 -7 -8 -9 -11 -10
+11 +9 +8 +7 +6 +5 +4 +3 +2 -1 -10
+11 +9 +8 +7 +6 +5 +4 +3 +2 +10 +1
</pre>