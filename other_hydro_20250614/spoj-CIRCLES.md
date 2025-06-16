<p>Little Gary plays the following video game. Circles pop up on the screen and disappear from it. When the screen flashes, Gary can draw a straight line on the screen and win as many points as there are circles intersected by the line. As a born-to-be-winner, Gary wants to maximize his score. Please, help him, and write a program that will determine the maximum number of points he can win each time the screen flashes.

</p><h3>Input</h3>
<p>The first line of the input contains <i>M</i> (<i>1</i> ¡Ü <i>M</i> ¡Ü <i>1000</i>), the number of events during the game. The next <i>M</i> lines contain descriptions of the events, one per line. They can be in one of the following three formats:
<br><br>
1 <i>x</i> <i>y</i> <i>r</i><br>
, representing a circle of radius <i>r</i> popping up with the position of its center at (<i>x</i>, <i>y</i>) in the plane
<br><br>
2 <i>i</i><br>
, representing a circle <i>i</i> disappearing, where circle <i>i</i> is the <i>i</i>th circle that popped up since the beginning of the game; and
<br><br>
3<br>
, representing the screen flashing.
<br><br>
<i>x</i>, <i>y</i>, and <i>r</i> are real numbers with at most two decimals, <i>-10<sup>6</sup></i> &lt; <i>x</i>, <i>y</i>, <i>r</i> &lt; <i>10<sup>6</sup></i>, <i>r</i> &gt; 0.
<br><br>
Notes:
</p><ul>
<li>A line intersects a circle if it has at least two common points with it.</li>
<li>At any time, no two Circles on the screen have a common point.</li>
<li>At any time, there is no line that "touches" more than two circles (a line touches a circle if they have exactly one common point).</li>
<li>At any time, there are no more than 100 circles on the screen.</li>
<li>Each <i>i</i> determines a circle that is on the screen at the moment of removal.</li>
<li>No circle is removed twice.</li>
</ul>

<h3>Output</h3>
<p>Each time the screen flashes, write an integer to a separate line, which is the maximum number of circles Gary can intersect.

</p><h3>Example</h3>

<pre><b>Input:</b>
9
1 3.00 0.00 1.00
1 -2.00 0.00 1.00
3
1 2.00 3.00 1.50
3
1 2.00 -4.00 1.00
3
2 3
3

<b>Output:</b>
2
2
3
2
</pre>