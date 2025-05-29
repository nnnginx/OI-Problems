<div style="text-align: left; margin: 10px 0px;"><div style="float: right; margin: 0px 0px 3px 10px;"><img src="/content/crazyb0y:CGW.jpg" width="250"></div><span>

<p>A defensive wall is a fortification used to protect a city or settlement from potential aggressors. From ancient to modern times, they were used to enclose settlements.</p>

<p>Generally, these are referred to as city walls or town walls. Even though, our ancestors decided to build a Great Wall to protect the northern borders of the Chinese Empire against invasion by various nomadic groups.</p>

<p>The map is given as an rectangle area of size <b>N</b>¡Á<b>M</b>. Each grid is an empty area, a city or an enemy. The Great Wall is a simple polygon build alone the edge of the grids, enclosing all the cities and keeping all the enemies out.</p>

<p>The Great Wall is not easy to build, so we should make the Great Wall as short as possible. Now it is your job to calculate the length of the shortest Great Wall so that it can protect all the cities from the enemies.</p>
</span></div>

<h3>Input</h3>
<p>The first line contains an integer <b>T</b> (1 ¡Ü T ¡Ü 50), indicating the number of test cases.</p>

<p>Each test case contains several lines. The first line contains two integer <b>H</b>, <b>W</b> (1 ¡Ü <b>H</b>, <b>W</b> ¡Ü 8), indicating the number of rows and columns of the map. The following <b>H</b> lines contains <b>W</b> chars, indicating the map. <tt>'o'</tt> represents a city, <tt>'.'</tt> represents a empty area and <tt>'x'</tt> represents an enemy.</p>
<p>You can assume that there will be at least one city on the map.</p>

<h3>Output</h3>
<p>For each test case in the input, print one line: <tt>"Case #X: Y"</tt>, where <b>X</b> is the test case number (starting with 1) and <b>Y</b> is the length of the shortest Great Wall (-1 if impossible).</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
3 3
.o.
.x.
o.o
4 4
....
.ox.
.xo.
....
5 5
.ooo.
.x...
..xoo
x.xoo
.ox.x

<b>Output:</b>
Case #1: 14
Case #2: -1
Case #3: 28
</pre>

<h3>Hint</h3>
<p>A simple polygon is a closed polygonal chain of line segments in the plane which do not have points in common other than the common vertices of pairs of consecutive segments.</p>

<p>The solution for the first test case in sample is shown in Figure 1.</p>
<p>There is no solution for the second test case because no matter how you build the Great Wall, it will always intersects with itself(Figure 2).</p><p>

</p><p><img src="/content/crazyb0y:CGW.png" align="middle" width="400"></p>