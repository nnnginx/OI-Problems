<p>The Czech Technical University is rather old - you already know that it celebrates 300 years
of its existence in 2007. Some of the university buildings are old as well. And the navigation
in old buildings can sometimes be a little bit tricky, because of strange long corridors that fork
and join at absolutely unexpected places.

</p><p>The result is that some first-graders have often difficulties finding the right way to their classes.
Therefore, the Student Union has developed a computer game to help the students to practice
their orientation skills. The goal of the game is to find the way out of a labyrinth. Your task is
to write a verification software that solves this game.

</p><p>The labyrinth is a 2-dimensional grid of squares, each square is either free or filled with a wall.
Some of the free squares may contain doors or keys. There are four different types of keys and
doors: blue, yellow, red, and green. Each key can open only doors of the same color.
You can move between adjacent free squares vertically or horizontally, diagonal movement is
not allowed. You may not go across walls and you cannot leave the labyrinth area. If a square
contains a door, you may go there only if you have stepped on a square with an appropriate key
before.

</p><h3>Input</h3>
<p>The input consists of several maps. Each map begins with a line containing two integer numbers
R and C (1 &lt;= R, C &lt;= 100) specifying the map size. Then there are R lines each containing C
characters. Each character is one of the following:<br>
Hash mark '#' Wall<br>
Dot '.' Free square<br>
Asterisk '*' Your position<br>
Uppercase letter 'B','Y','R','G' Blue, yellow, red or green door<br>
Uppercase X 'X' Exit<br>

</p><p>Note that it is allowed to have
* more than one exit,<br>
* no exit at all,<br>
* more doors and/or keys of the same color, and<br>
* keys without corresponding doors and vice versa.<br>

</p><p>You may assume that the marker of your position ("*") will appear exactly once in every map.
There is one blank line after each map. The input is terminated by two zeros in place of the
map size.

</p><h3>Output</h3>
<p>For each map, print one line containing the sentence "Escape possible in S steps.", where
S is the smallest possible number of step to reach any of the exits. If no exit can be reached,
output the string "The poor student is trapped!" instead.
One step is defined as a movement between two adjacent cells. Grabbing a key or unlocking
a door does not count as a step.

</p><h3>Example</h3>
<pre><b>Input:</b>
1 10
*........X

1 3
*#X

3 20
####################
#XY.gBr.*.Rb.G.GG.y#
####################

0 0

<b>Output</b>
Escape possible in 9 steps.
The poor student is trapped!
Escape possible in 45 steps.

</pre>