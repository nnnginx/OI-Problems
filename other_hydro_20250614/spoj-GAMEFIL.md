<p>
Almost anyone who has ever taken a class in computer science is familiar with the ¡°Game of Life,¡± John
Conway¡¯s cellular automata with extremely simple rules of birth, survival, and death that can give rise
to astonishing complexity.

</p><p></p><p>
The game is played on a rectangular field of cells, each of which has eight neighbors (adjacent cells). A
cell is either occupied or not. The rules for deriving a generation from the previous one are:

</p><ul>
<li> If an occupied cell has 0, 1, 4, 5, 6, 7, or 8 occupied neighbors, the organism dies (0, 1: of loneliness;
4 thru 8: of overcrowding).
</li><li> If an occupied cell has two or three occupied neighbors, the organism survives to the next gener-
ation.
</li><li> If an unoccupied cell has three occupied neighbors, it becomes occupied (a birth occurs).
</li></ul>

<p></p><p>
One of the major problems researchers have looked at over the years is the existence of so-called ¡°Garden
of Eden¡± configurations in the Game of Life ¡ª configurations that could not have arisen as the result of
the application of the rules to some previous configuration. We¡¯re going to extend this question, which
we¡¯ll call the ¡°Game of Efil¡±: Given a starting configuration, how many possible parent configurations
could it have? To make matters easier, we assume a finite grid in which edge and corner cells ¡°wrap
around¡± (i.e., a toroidal surface). For instance, the 2 by 3 configuration:

</p><p></p><p>
<img src="/content/steinersp:efil1.png" alt="subir imagenes" border="0">
</p><p></p><p>
has exactly three possible parent configurations; they are:

</p><p></p><p>
<img src="/content/steinersp:efil2.png" alt="subir imagenes" border="0">

<img src="/content/steinersp:efil3.png" alt="subir imagenes" border="0">

<img src="/content/steinersp:efil4.png" alt="subir imagenes" border="0">

</p><p></p><p>
You should note that when counting neighbors of a cell, another cell may be counted as a neighbor
more than once, if it touches the given cell on more than one side due to the wrap around. This is the
case for the configurations above.

</p><p>
</p><h3>Input</h3>
<p>
There will be multiple test cases. Each case will start with a line containing a pair of positive integers <i>m</i>
and <i>n</i>, indicating the number of rows and columns of the configuration, respectively. The next line will
contain a nonnegative integer <i>k</i> indicating the number of ¡°live¡± cells in the configuration. The following
<i>k</i> lines each contain the row and column number of one live cell, where row and column numbering
both start at zero. The final test case is followed by a line where <i>m</i> = <i>n</i> = 0 ¡ª this line should not be
processed. You may assume that the product of <i>m</i> and <i>n</i> is no more than 16.

</p><h3>Output</h3>
<p>
For each test case you should print one line of output containing the case number and the number of
possible ancestors. Imitate the sample output below. Note that if there are 0 ancestors, you should
print out

</p><p></p><p>
</p><pre><b>Garden of Eden.</b></pre>

<h3>Example</h3>
<pre><b>Input:</b>
2 3
2
0 0
0 1
3 3
4
0 0
0 1
0 2
1 1
3 3
5
0 0
1 0
1 2
2 1
2 2
0 0

<b>Output:</b>
Case 1: 3 possible ancestors.
Case 2: 1 possible ancestors.
Case 3: Garden of Eden.
</pre>