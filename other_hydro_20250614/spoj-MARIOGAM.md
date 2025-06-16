<p>Mario lives in an <i>N x M</i> maze grid.  In this maze there are coin
boxes, monsters, pipe systems, and walls.  Whenever Mario enters a
cell
containing a coin box, he jumps to hit the box and gets as many coins
as there are in the box (coin boxes do not disappear or lose coins
after being hit).  When Mario enters a cell with a monster, he loses a
life.  Pipe systems are like teleporters: for each system there is
exactly one exit with at least one (but possibly several) entrances
leading to that
exit.  When Mario walks into the entrance to a pipe system he is
teleported to that pipe system's unique exit.  Walking into a pipe
system's exit does nothing special.  Finally, Mario cannot walk into
walls.

</p><p>Mario decides to play a game.  In the beginning of the game he
starts with three lives at some given position, and at each time step
he looks at all neighboring cells (excluding walls) and chooses one
neighboring cell uniformly at random to walk to (x neighbors y if x is directly above, below, to the left, or to the right of y).  If Mario has no
non-wall neighboring cells then he stays at his current location.  The
game is over when either
Mario is out of lives or it is impossible for him to collect more
coins.  Help Mario figure out the expected number of coins he will
earn in one play of the game.

</p><h3>Input</h3>
<p>The first line of the input is "<i>N M</i>" (1 ¡Ü <i>N,M</i> ¡Ü 15), giving the
dimensions of the maze.  What follows are <i>N</i> lines, each of which are
<i>M</i> characters in length.  The ith line displays the contents of the
cells in the ith row of the maze.  Mario starts in the unique
cell with
an '$' (which, beside holding Mario, is otherwise an empty cell).
Cells with monsters are designated with '!'.  Cells with
coin boxes are represented by a number between <i>0</i> and <i>9</i>
(inclusive), which is the number of coins in that coin box.  Each
pipe system is associated with a distinct letter between 'a' and 'z'
(inclusive).  A pipe system's entrances are designated with lower
case letters,
and the unique exit for a given pipe system has the corresponding
capitalized letter
(e.g. a pipe system with entrances labeled 'c' has exactly one exit,
and it is labeled 'C').  Every pipe
system appearing in the maze is
guaranteed to have exactly one exit and at least one entrance.  The
character '#' designates a wall, and '.' designates an empty cell
that Mario can just walk through.

</p><h3>Output</h3>
<p>If the expected number of coins Mario collects is infinite, output
-1.  Otherwise, output a
single real number, the expected number of
coins Mario collects before the game is over.  Your answer should be
accurate to within either an absolute or relative error of 10<sup>-6</sup> of the actual answer.
Your output should be followed by a newline.

</p><h3>Example</h3>

<pre><b>Input:</b>
2 3
$1!
a.A

<b>Output:</b>
3.000000000
</pre>