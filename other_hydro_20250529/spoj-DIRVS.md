<p>
Building the GSM network is a&nbsp;very expensive and complex task. Moreover,
after the <em>Base Transceiver Stations</em> (<em>BTS</em>) are built and
working, we need to perform many various measurements to determine the state
of the network, and propose effective improvements to be made.


</p><p>
The ACM technicians have a&nbsp;special equipment for measuring the strength of
electro-magnetic fields, the transceivers' power and quality of the signal.
This equipment is packed into a&nbsp;huge knapsack and the technician must move
with it from one BTS to another. Unfortunately, the knapsack have not enough
memory for storing all of the measured values. It has a&nbsp;small cache only,
that can store values for several seconds. Then the values must be
transmitted to the BTS by an&nbsp;infrared connection (IRDA). The IRDA needs
direct visibility between the technician and the BTS.

</p><p>
Your task is to find the path between two neighbouring BTSes such that at
least one of those BTSes is always visible.

</p><p>
</p><h3>Input</h3>

<p>
There is a&nbsp;single positive integer <var>T</var> on the first line of input (equal to about 500). It stands
for the number of test cases to follow. Each test case consists of a&nbsp;town
description. For simplicity, a&nbsp;town is modelled as a&nbsp;rectangular grid of

<var>P x Q</var> square fields. Each field is exactly 1&nbsp;metre wide. For each
field, a&nbsp;non-negative integer <var>Z</var><sub><var>i</var>,<var>j</var></sub> is given, representing the height of
the terrain in that place, in metres. That means the town model is made of
cubes, each of them being either solid or empty. There are no "half solid"
cubes.

</p><p>
The first line of each test case contains two integer numbers <var>P</var> and <var>Q</var>,
separated by a&nbsp;single space, 
1 &lt;= <var>P</var>,<var>Q</var> &lt;= 200. Then there are <var>P</var> lines
each containing <var>Q</var> integer numbers separated by a&nbsp;space. These numbers are

<var>Z</var><sub><var>i</var>,<var>j</var></sub>, where 
1 &lt;= <var>i</var> &lt;= <var>P</var>, 
1 &lt;= <var>j</var> &lt;= <var>Q</var> and

0 &lt;= <var>Z</var><sub><var>i</var>,<var>j</var></sub> &lt;= 5000. After the terrain
description, there are four numbers 

<var>R</var><sub>1</sub>, <var>C</var><sub>1</sub>, <var>R</var><sub>2</sub>, <var>C</var><sub>2</sub> on the last line of
each test case. These numbers represent position of two
BTSes, 
1 &lt;= <var>R</var><sub>1</sub>,<var>R</var><sub>2</sub> &lt;= <var>P</var>, 
1 &lt;= <var>C</var><sub>1</sub>,<var>C</var><sub>2</sub> &lt;= <var>Q</var>. The first coordinate
(<var>R</var>) determines the row of the town, the second coordinate determines the
column.


</p><p>
The technician is moving in steps (<em>steps</em> stands for
<em>Standard Technician's Elementary Positional Shift</em>). Each step is made
between two neighbouring square fields. That means the step is always in
North, South, West or East direction. It is not possible to move diagonally.
The step between two fields <var>A</var> and <var>B</var> (step from <var>A</var> to <var>B</var>) is allowed
only if the height of the terrain in the field <var>B</var> is not very different from
the height in the field <var>A</var>. The technician can climb at most 1&nbsp;metre up or
descend at most 3&nbsp;metres down in a&nbsp;single step.


</p><p>
At the end of each step, at least one of the two BTSes must be visible.
However, there can be some point "in the middle of the step" where no BTS
is visible. This is OK and the data is handled by the cache. The BTS is
considered visible, if there is a&nbsp;direct visibility between the unit cube
just above the terrain on the BTSes coordinates and the cube just above the
terrain on the square field, where the technician is. Direct visibility
between two cubes means that the line connecting the centres of the two cubes
does not intersect any solid cube. However, the line can touch any number of
solid cubes. In other words, consider both the BTS and the technician being
points exactly half metre above the surface and in the centre of the
appropriate square field.

</p><p>
Note that the IRDA beam can go between two cubes that touch each other by
their edge, although there is no space between them. It is because such
a&nbsp;beam touches both of these two cubes but does not intersect any of
them. See the last test case of the sample input for an&nbsp;example of such
a&nbsp;situation.

</p><p>
</p><h3>Output</h3>

<p>
You are to find the shortest possible path from BTS (<var>R</var><sub>1</sub>, <var>C</var><sub>1</sub>) to BTS (<var>R</var><sub>2</sub>, <var>C</var><sub>2</sub>), meeting the above criteria. All
steps must be done between neighbouring fields, the terrain must not elevate
or descend too much, and at the end of each step, at least one BTS must be
visible.

</p><p>
For each test case, print one line containing the sentence
<tt>The shortest path is </tt><var>M</var><tt> steps long.</tt>, where <var>M</var> is the number of
steps that must be made. If there is no such path, output the sentence

<tt>Mission impossible!</tt>.

</p><h3>Example</h3>
<p>Sample Input:</p>

<pre><tt>4
5 5
8 7 6 5 4
2 2 2 2 2
2 2 2 2 2
2 2 2 2 2
2 2 2 2 2
1 1 5 1
5 8
2 2 2 2 2 2 2 2
2 2 2 2 2 2 2 2
2 2 2 2 2 2 2 2
9 9 9 9 9 9 9 2
2 2 2 2 2 2 2 2
1 2 5 1
5 8
2 2 2 2 2 2 2 2
2 2 2 2 2 2 2 2
2 2 2 2 2 2 2 2
9 9 9 9 9 9 9 2
2 2 2 2 2 2 2 2
1 5 5 1
6 12
5 5 5 5 1 5 5 5 5 5 5 5
5 5 5 5 1 5 5 5 5 5 5 5
5 5 5 5 9 5 5 5 5 5 5 5
5 9 1 5 5 5 5 5 5 5 5 5
5 5 9 5 5 5 5 5 5 5 5 5
5 5 9 5 5 5 5 5 5 5 5 5
6 1 3 12
</tt></pre>

<p>Sample Output:</p>

<pre><tt>The shortest path is 10 steps long.
Mission impossible!
The shortest path is 14 steps long.
The shortest path is 18 steps long.
</tt></pre>