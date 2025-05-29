<p>So called <i>commedia dell' arte</i> is a theater genre first
played in Italy at the beginning of the sixteenth century. It was inspired
with the Roman Theater. The play had no fixed script and the actors (also
called <i>performers</i>) had to improvise a lot. There were only a simple
directions by the author like "enter the stage and make something funny" or
"everyone comes on stage and everything is resolved happily". You can see it
might be very interesting to play the commedia dell' arte. Therefore
the ACM want to put a new play on a stage, which was completely unknown
before. The main hero has a puzzle that takes a very important role in the
play and gives an opportunity of many improvisations.

The puzzle is the worldwide known <i>Lloyd's Fifteen Puzzle</i>. ACM wants
to make the play more interesting so they want to replace the
"standard" puzzle with a three-dimensional one. The puzzle consists
of a cube containing <var>M<sup>3</sup></var> slots. Each slot except one
contains a cubic tile (one position is free).
The tiles are numbered from <var>1</var> to <var>M<sup>3</sup>-1</var>.
The goal of the puzzle is to get the original ordering of
the tiles after they have been randomly reshuffled.  The only allowed
moves are sliding a neighbouring tile into the free position along one
of the three principal directions. Original configuration is when slot
with coordinates <var>(x,y,z)</var> from <var>{0,...,M-1}<sup>3</sup></var>
contains tile number <var>z.M<sup>2</sup>+y.M+x+1</var> and slot
<var>(M-1,M-1,M-1)</var> is free.

</p><p>You are to write a program to determine whether it is possible 
to solve the puzzle or not.


</p><h3>Input</h3>

<p>The input consists of <var>N</var> cases. The first line of the input
contains only positive integer <var>N</var>. Then follow the cases. The
first line of each case contains only one integer <var>M</var>, <var>1 &lt;=
M &lt;= 100</var>. It is the size of 3D puzzle cube.  Then follow
<var>M</var> lines, each contains exactly <var>M<sup>2</sup></var> numbers
on the tiles for one layer. First is the layer on the top of the cube and
the last one on the bottom. In each layer numbers are arranged from the left
top corner linewise to the right bottom corner of the layer. In other words,
slot with coordinates <var>(x,y,z)</var> is described by the
<var>(x+M.y+1)</var>-th number on the <var>(z+1)</var>-th line.
Numbers are separated by space.  Number <var>0</var> means free position.


</p><h3>Output</h3>

<p>For each case, print exactly one line. 
If the original configuration can be reached by sliding the tiles,
print the sentence '<tt>Puzzle can be solved.</tt>'. Otherwise, print the
sentence '<tt>Puzzle is unsolvable.</tt>'.


</p><h3>Example</h3>
<pre>Sample input:

2
2
1 2 3 4
5 7 6 0
2
2 1 3 5
4 6 0 7

Sample output:

Puzzle is unsolvable.
Puzzle can be solved.
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>