<p>In a game there are infinite number of levels. In order to go to the next level,a player has to clear all the preceding levels. A player cant go further,if  he fails to clear the level. Each  player has a probability p of clearing the level (which is independent of the other players and the level number). For  example, if p =1/2 there is a probability 2^(-n-1) that a particular game will have exactly n levels cleared.A player will get Gold medal if he clears the maximum number of levels. If the maximum number of levels reached is common between two or more players, then no one wins the gold medal.What is the probability that  a Gold medal is given to any player?</p>
<h3>Input</h3>
<p>T number of test cases each case follow<br>p n m . probability of clearing level for each player, number of player, number of levels in game</p>
<h3>Output</h3>
<p>T line each probability that gold medal is given round off to 4 significant digits</p>
<p>limit:</p>
<p>1&lt;=T&lt;10000<br> 1&lt;=n&lt;1000<br> 1&lt;=m&lt;100<br> 0&lt;=p&lt;=1.0</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>6<br>0.43 3 2<br>0.5 3 4<br>0.2 3 4<br>0.1 4 5<br>0.9 3 3<br>1.0 4 4<br><strong>Output:</strong>
0.4490<br>0.6244<br>0.4184<br>0.3014<br>0.0275<br>0.0000</pre>