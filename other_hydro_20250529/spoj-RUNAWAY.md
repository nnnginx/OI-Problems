<p align="justify">
One of the traps we will encounter in the Pyramid is located in the Large Room.
A lot of small holes are drilled into the floor. They look completely harmless
at the first sight. But when activated, they start to throw out very
hot java, uh ... pardon, lava. Unfortunately, all known paths to the Center
Room (where the Sarcophagus is) contain a&nbsp;trigger that activates the
trap. The ACM were not able to avoid that. But they have carefully monitored
the positions of all the holes. So it is important to find the place in the
Large Room that has the maximal distance from all the holes. This place is
the safest in the entire room and the archaeologist has to hide there.

</p><h3>Input</h3>

<p align="justify">The input consists of <var>T</var> test cases. The number of them (<var>T</var>) is
given on the first line of the input file.  Each test case begins with a
line containing three integers <var>X</var>, <var>Y</var>, <var>M</var> separated by space. The numbers
satisfy conditions: 
<var>1 &lt;= X,Y &lt;=10000</var>, <var>1 &lt;= M &lt;= 1000</var>. The
numbers <var>X</var> and <var>Y</var>indicate the dimensions of the Large
Room which has a&nbsp;rectangular
shape. The number <var>M</var> stands for the number of holes. Then exactly <var>M</var> lines
follow, each containing two integer numbers <var>U<sub>i</sub></var> and <var>V<sub>i</sub></var>
(<var>0 &lt;= U<sub>i</sub> &lt;= X</var>,
<var>0 &lt;= V<sub>i</sub> &lt;= Y</var>) indicating the coordinates of one
hole. There may be several holes at the same position.

</p><h3>Output</h3>
<p align="justify">
Print exactly one line for each test case. The line should contain the
sentence "<code>The safest point is (<var>P</var>, <var>Q</var>).</code>"
where <var>P</var> and <var>Q</var>are the coordinates of the point in the
room that has the maximum
distance from the nearest hole, rounded to the nearest number with exactly
one digit after the decimal point (0.05 rounds up to 0.1).

</p><h3>Example</h3>

<pre>Sample Input:
3
1000 50 1
10 10
100 100 4
10 10
10 90
90 10
90 90
3000 3000 4
1200 85
63 2500
2700 2650 
2990 100

Sample output:
The safest point is (1000.0, 50.0).
The safest point is (50.0, 50.0).
The safest point is (1433.0, 1669.8).
</pre>