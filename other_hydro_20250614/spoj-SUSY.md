<p>Susy is a beautiful and smart student. She is an expert &nbsp;solving puzzle games, specially mazes, and such talent has given her several prizes from various competitions, where her speed and skills are tested.
</p><p>Right now, she is participating in an special puzzle contests, and her jealous rival, Angelica, is participating too.
</p><p>At this moment, they are in a tie, and in order to break this tie the judges have prepared a special round with a special game. The rules of this game are the following:
</p><p>-The game consists of a table with walls, like a maze. Also, there are some special objects, the Magic Stones. To win the game, the player must take all the stones present in the table.
</p><p>-There are four valid movements: Up, Down, Left and Right. Nevertheless, once the player choose a movement from his current position, he cannot stop moving in that direction until he crash with a wall in the maze. Obviously, the player cannot leave the table, so the limits of the table are considered walls too.
</p><p>-As there can be many solutions, the judges want the optimal one, which mean the least number of moves.
</p><p>This is not problem for Susy, but Angelica is having a really bad time with this game. Jealously, Angelica secretly took Susy's solution and cut it in many pieces (She is not very intelligent. She could copy the solution instead but her anger blinded her).
</p><p>Time is running out, and Susy doesn't have the time required to solve the puzzle again. Fortunately, the participants can ask a friend to help with just one puzzle, and she knows something the judges don't, your programming skills.
</p><p>Now, she is calling you! Write a program to solve the maze with the least moves possible! Help Susy!

</p><p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The input begins with two integer numbers, R and C, the number of rows and columns of the table respectively.</p>
<p>Next, there will be R lines with C characters each, representing the maze. Each maze will contain only following characters:<br>
"." - free space,<br>
"#" - wall,<br>
"S" - initial position of the player,<br>
"*" - magic stone.
</p><p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>The output consists of 2 lines. The first must contain one only number S. S is the optimal solution of the game.
</p><p>The next line consists of S strings separated with a "-". These strings are "Up", "Down", "Left" and "Right". The full string represents the movements done in the optimal solution.
</p><p>If there is more than one optimal solution, you must print the lexicographically smallest one.
</p><p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 6
*S....
....#.
.##...
**....
.#.*#.


<strong>Output:</strong>
7
Down-Right-Down-Left-Up-Left-Up</pre>
<pre><strong>Constraints:</strong>
2&lt;=(r,c)&lt;=20
There will be no more than 13 magic stones in the maze.
<strong>NOTE:</strong>
There will always be a solution for the given maze.</pre>