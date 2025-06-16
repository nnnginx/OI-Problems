<p>Lizarb's national soccer team undoubtedly belongs to the group of favourites to win the World Cup at the upcoming championship. Their greatest advantages are their excellent dribbling skills   and the ball passing precision. Particularly, each player can pass the ball to every other player  on the playing field at any distance. The team's captain, Oicul, claims that an exercise which certainly  has a substantial effect on the team's soccer skills is the so-called "Two-ball Game".</p>
<p>In the two-ball game, <em>n &gt; 4</em> kickers are positioned on the playing field and do not move (i.e.\ change their locations) during the game.  Four of the players are distinguished: two of them, denoted as <em>s<sub>1</sub></em> and <em>s<sub>2</sub></em>, are called  starting players, and two others, denoted as <em>t<sub>1</sub></em> and <em>t<sub>2</sub></em>, are called terminal players. At the beginning, player <em>s<sub>1</sub></em> has got a white ball and <em>s<sub>2</sub></em> possesses a black ball. Then each starting  player can kick the ball directly to the corresponding terminal player but he can also kick the  ball to any other player on the field and this player can pass the ball to the next one, and so on.  The aim is that at the end the white ball is in possession of <em>t<sub>1</sub></em> and the black ball in possession  of <em>t<sub>2</sub></em>. So, it seems the game is quite simple. However, to avoid ball collisions,  the constraint of the game is that no ball trajectories cross each other and that no player  (including starting and terminal ones) has more than one ball contact. For simplicity, we assume the  trajectory of a ball moving from one player to the next one is a line segment.</p>
<p>Lizarb's national soccer team observed that for some locations of kickers the two-ball game is possible but for some others it is impossible. The figure below shows two example locations: to the left, playing two-ball game is impossible; to the right, playing the game is possible.</p>
<p><img src="../../../content/ak15:tbgame.png" alt="example image" width="85%"></p>
<p>Your task is to write a program that checks if for given player locations the two-ball game is possible or not.</p>
<h3>Input</h3>
<p>Each input starts with a single integer that gives the number of cases that follow.  The firsts line of each case contains the number of players <em>n</em>, with <em>4 �� n �� 100000</em> followed by <em>n</em> lines that describe the coordinates of the players. All coordinates are pairwise different and  the points determined by the coordinates are <em>not</em> collinear (recall, three or more points are said to be collinear if they lie on a single straight line).  The first coordinate describes the location  of <em>s<sub>1</sub></em>, the second the location of <em>t<sub>1</sub></em>, the third coordinate describes the location  of <em>s<sub>2</sub></em>, and the fourth the location of <em>t<sub>2</sub></em>. The remaining coordinates describe  positions of other players of the team.</p>
<h3>Output</h3>
<p>For each case, your algorithm has to output a line containing POSSIBLE if it is  possible to play the game and IMPOSSIBLE, otherwise.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>

2
5
2.01 0.02
1.04 3.02
0.01 0.99
4.1  3.2
2.1  2.01
5
2.01 0.02
1.04 3.02
0.01 0.99
2.1  2.01
4.1  3.2

<strong>Output:</strong>
IMPOSSIBLE
POSSIBLE
</pre>