## Description

<div><p>This afternoon, you decided to enjoy the first days of Spring by taking a walk outside. As you come near the Quidditch field, you hear screams. Once again, there is a conflict about the score: the two teams are convinced that they won the game! To prevent this problem from happening one more time, you decide to get involved in the refereeing of the matches.</p><p>Now, you will stay in the stadium to watch the game and count the score. At the end of the game, you will decide the winner.</p><p>Today, two teams are competing: the red Gryffindor (<span class="tex-font-style-tt">R</span>) and the blue Ravenclaw (<span class="tex-font-style-tt">B</span>) team. Each team is composed of $P$ players ($1 \leq P \leq 10$).</p><p>The field is a rectangle of $N$ lines and $M$ columns ($3 \leq N, M \leq 99$, $N$ and $M$ are odd). All the positions are integers, and several entities are allowed to be at the same position in the field. At the beginning of the game, the field contains goals for the two teams (each team can own between one and five goals), the players, and exactly one Quaffle. Other types of balls will be available in the harder versions of the problem.</p><p>A game is composed of $T$ steps ($0 \leq T \leq 10000$). At each step, one entity on the field (a player or a ball) performs one action. All entities can move. A player can also catch a ball or throw the Quaffle that it is carrying. To catch a ball, a player must be located on the same cell as it. The Quaffle does not perform any action while it is being carried; it only follows the movements of the player. If a player carrying the Quaffle decides to throw it, the Quaffle is simply put at the current position of the player.</p><p>To win a point, a player must leave the Quaffle at a goal of the other team. When it does, the team of the player wins one point, and the Quaffle instantly moves to the middle of the field (the cell at the $(M+1)/2$-th column of the $(N+1)/2$-th line of the field, starting from 1). There is no goal in the middle of the field. If a player puts the ball in its own goal, the other team wins the point.</p></div><div class="input-specification"><p>On the first line, the integers $N$ and $M$.</p><p>The description of the field follows: $N$ lines of $M$ pairs of characters separated by spaces. Each pair of characters represents a position on the field. It can be either: </p><ul> <li> <span class="tex-font-style-tt">..</span> to represent an empty cell </li><li> <span class="tex-font-style-tt">R0</span>, ..., <span class="tex-font-style-tt">R9</span>, <span class="tex-font-style-tt">B0</span>, ..., <span class="tex-font-style-tt">B9</span> to represent a player. The first character is the team of the player, and the second is the number of the player in the team. Each pair of characters is unique, but it is not guaranteed that all the pairs appear in the grid. </li><li> <span class="tex-font-style-tt">RG</span> or <span class="tex-font-style-tt">BG</span> to represent a goal. The blue team tries to put the ball in a red goal (<span class="tex-font-style-tt">RG</span>) while the red team tries to put the ball in a blue goal (<span class="tex-font-style-tt">BG</span>). </li><li> <span class="tex-font-style-tt">.Q</span> to represent the Quaffle, which is the ball that the players use to score goals. </li></ul><p>The next line contains $T$, the number of steps that compose the game. $T$ lines follow, each describing one action. It contains several pieces of information separated by a space. First, a pair of characters representing the entity that must perform the action. Second, the description of the action: </p><ul> <li> <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span> indicate that the entity moves on the grid. It can move to the top of the grid (<span class="tex-font-style-tt">U</span>), to the bottom (<span class="tex-font-style-tt">D</span>), to the left (<span class="tex-font-style-tt">L</span>), or to the right (<span class="tex-font-style-tt">R</span>). Each entity moves by only one cell at a time. </li><li> <span class="tex-font-style-tt">C</span> indicates that the player catches the ball (only a player can catch a ball). Then, there is a space followed by a pair of characters: the description of the ball caught by the player. This information is needed since in the next versions of the problem, several balls may be in the same cell. </li><li> <span class="tex-font-style-tt">T</span> indicates that the player throws the Quaffle that it is carrying. </li></ul><p>All the actions performed by the entities are guaranteed to be valid: the players stay in the field, don't catch a ball if they are not in the same cell, don't release the Quaffle if they are not carrying it, ...</p></div><div class="output-specification"><p>You must output the description of the main events of the game, one event per line. More precisely:</p><ul> <li> Each time a team scores, you must print <span class="tex-font-style-tt">t RED GOAL</span> or <span class="tex-font-style-tt">t BLUE GOAL</span>, depending on the team who scored, where <span class="tex-font-style-tt">t</span> is the current time (the position of the action in the list of actions, starting from 0). In the case where a player scores in the wrong goal (a red player scores in the red goal, or a blue player scores in the blue goal), you must print the name of the team who wins one point, that is, the other team. </li></ul><p>The events must be printed in ascending order of <span class="tex-font-style-tt">t</span>.</p><p>At the end of the game, you must print the final score as: <span class="tex-font-style-tt">FINAL SCORE: r b</span>, where <span class="tex-font-style-tt">r</span> is the score of the red team and <span class="tex-font-style-tt">b</span> is the score of the blue team.</p></div>

## Input

<p>On the first line, the integers $N$ and $M$.</p><p>The description of the field follows: $N$ lines of $M$ pairs of characters separated by spaces. Each pair of characters represents a position on the field. It can be either: </p><ul> <li> <span class="tex-font-style-tt">..</span> to represent an empty cell </li><li> <span class="tex-font-style-tt">R0</span>, ..., <span class="tex-font-style-tt">R9</span>, <span class="tex-font-style-tt">B0</span>, ..., <span class="tex-font-style-tt">B9</span> to represent a player. The first character is the team of the player, and the second is the number of the player in the team. Each pair of characters is unique, but it is not guaranteed that all the pairs appear in the grid. </li><li> <span class="tex-font-style-tt">RG</span> or <span class="tex-font-style-tt">BG</span> to represent a goal. The blue team tries to put the ball in a red goal (<span class="tex-font-style-tt">RG</span>) while the red team tries to put the ball in a blue goal (<span class="tex-font-style-tt">BG</span>). </li><li> <span class="tex-font-style-tt">.Q</span> to represent the Quaffle, which is the ball that the players use to score goals. </li></ul><p>The next line contains $T$, the number of steps that compose the game. $T$ lines follow, each describing one action. It contains several pieces of information separated by a space. First, a pair of characters representing the entity that must perform the action. Second, the description of the action: </p><ul> <li> <span class="tex-font-style-tt">U</span>, <span class="tex-font-style-tt">D</span>, <span class="tex-font-style-tt">L</span>, <span class="tex-font-style-tt">R</span> indicate that the entity moves on the grid. It can move to the top of the grid (<span class="tex-font-style-tt">U</span>), to the bottom (<span class="tex-font-style-tt">D</span>), to the left (<span class="tex-font-style-tt">L</span>), or to the right (<span class="tex-font-style-tt">R</span>). Each entity moves by only one cell at a time. </li><li> <span class="tex-font-style-tt">C</span> indicates that the player catches the ball (only a player can catch a ball). Then, there is a space followed by a pair of characters: the description of the ball caught by the player. This information is needed since in the next versions of the problem, several balls may be in the same cell. </li><li> <span class="tex-font-style-tt">T</span> indicates that the player throws the Quaffle that it is carrying. </li></ul><p>All the actions performed by the entities are guaranteed to be valid: the players stay in the field, don't catch a ball if they are not in the same cell, don't release the Quaffle if they are not carrying it, ...</p>

## Output

<p>You must output the description of the main events of the game, one event per line. More precisely:</p><ul> <li> Each time a team scores, you must print <span class="tex-font-style-tt">t RED GOAL</span> or <span class="tex-font-style-tt">t BLUE GOAL</span>, depending on the team who scored, where <span class="tex-font-style-tt">t</span> is the current time (the position of the action in the list of actions, starting from 0). In the case where a player scores in the wrong goal (a red player scores in the red goal, or a blue player scores in the blue goal), you must print the name of the team who wins one point, that is, the other team. </li></ul><p>The events must be printed in ascending order of <span class="tex-font-style-tt">t</span>.</p><p>At the end of the game, you must print the final score as: <span class="tex-font-style-tt">FINAL SCORE: r b</span>, where <span class="tex-font-style-tt">r</span> is the score of the red team and <span class="tex-font-style-tt">b</span> is the score of the blue team.</p>





```input1|
5 5
.. R1 .. B1 ..
RG .. .. .. BG
RG R0 .Q B0 BG
RG .. .. .. BG
.. R2 .. B2 ..
13
B2 U
B2 U
B2 L
B2 C .Q
B2 L
B2 L
B2 T
R0 R
R0 C .Q
R0 D
R0 R
R0 R
R0 T
```




```input2|
3 5
.. .. R0 .. ..
RG .. .Q .. BG
.. .. B0 .. ..
12
R0 D
R0 C .Q
R0 R
R0 T
R0 D
B0 R
B0 U
B0 C .Q
B0 L
B0 L
B0 L
B0 T
```




```input3|
3 5
.. .. R0 .. ..
RG .. .Q .. BG
.. .. B0 .. ..
5
R0 D
R0 C .Q
R0 L
R0 L
R0 T
```




```output1
6 BLUE GOAL
12 RED GOAL
FINAL SCORE: 1 1
```




```output2
11 BLUE GOAL
FINAL SCORE: 0 1
```




```output3
4 BLUE GOAL
FINAL SCORE: 0 1
```



## Note

<p>In the first example, a blue player goes to the middle of the grid, at the position of the Quaffle. He takes it, goes to the goal of the red team, and lets the ball there. He scores! The ball gets back to the middle of the field, a red player takes it and scores too.</p><p>In the second example, the red player takes the Quaffle, move it and throw it. The blue player catches the ball, goes to the red goal and scores.</p><p>In the third example, the red player takes the ball and scores in the goal of their own team: the blue team wins a point.</p>
