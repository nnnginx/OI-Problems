<p>The famous witch is back. After killing an incredible amount of monsters in order to find a
hidden treasure, Zak Galou decided to buy vineyards in Burgundy and retired. Everything was
calm in his new life, until the day that his farm tractor stopped working.

</p><p></p><p>
His tractor��s engine works based on a mechanism of gears. The engine can be represented by
a bidimensional grid. At most one gear can be attached to each position of the grid. All the
gears are identical and can mesh with adjacent gears. In this grid, a gear can have up to six
other adjacent gears, see figure below:

</p><p></p><p>
</p><center><img src="/content/steinersp:galou1.jpg" alt="subir imagenes" border="0"></center>

<p></p><p>
Under normal utilization, when the tractor is started, some of the gears are initially activated
and try to turn clockwise. When a gear tries to turn in one direction, all the adjacent gears try
to turn in the opposite direction.

</p><p></p><p>
When Zak Galou opened his engine he noticed that it had been sabotaged (probably by a
jealous treasure hunter who was not able to find the treasure). Some of the gears were removed
from the engine and others have been added to it. As a consequence, some of the gears were
immobile. A gear can be immobile either if it is free or if it is blocked. A gear is free when it is
not an initially activated gear and no adjacent gear is trying to turn. A gear is blocked when it
is trying to turn in both directions at the same time. For example, consider that there are three
gears in the engine as shown in the figure below. If any of the gears is initially activated when
the tractor is started, all of them will be blocked. If none of the gears are initially activated,
all of them will be free.

</p><p></p><p>
</p><center><img src="/content/steinersp:galou2.jpg" alt="subir imagenes" border="0"></center>

<p></p><p>
As a part of the work of fixing his tractor, Zak Galou asks for your help to solve the following
problem. Given the description of the engine and the gears that are initially activated in the
clockwise direction, he wants to know for each gear, what is its state when the tractor is started:
turn clockwise, turn counter-clockwise, free or blocked.

</p><h3>Input</h3>
<p>The input contains several test cases. The first line of a test case contains two integers R and
C, separated by a single space, representing respectively the number of rows and columns of the
engine grid (1 &lt;= R,C &lt;= 100). The next R lines describe the engine. The i-th line represents
the i-th row of the engine and contains C characters. The character ��.�� indicates that there
is no gear in the corresponding position, the character ��*�� indicates that there is a gear that
<i>is not</i> initially activated when the engine is started and an ��I�� indicates that there is a gear
that <i>is</i> initially activated when the engine is started. Notice that, for simplicity reasons, the
parallelogram representing the engine grid is described in the input as if it was a rectangle with
each row left aligned. The end of input is indicated by R = C = 0

</p><h3>Output</h3>
<p>For each test case, your program must output R + 1 lines. The first line must be empty; each
of the following R lines must have C characters. The characters printed must represent the
state of each position of the grid when the engine is started. Print a ��.�� if there is no gear in
the position; a ��(�� if there is a gear turning in the clockwise direction; a ��)�� if there is a gear
turning in the counter-clockwise direction, an uppercase ��F�� if there is a gear that is free and
an uppercase ��B�� if there is a blocked gear.
</p><h3>Example</h3>

<pre><b>Input:</b>
4 3
...
.*.
.I.
...
4 4
....
.**.
.I..
..*.
0 0

<b>Output:</b>
...
.).
.(.
...
....
.BB.
.B..
..F.
</pre>