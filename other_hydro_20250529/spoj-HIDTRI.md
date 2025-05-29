<p>
Assume that each `<tt>0</tt>' or `<tt>1</tt>' in the array represents a point on a plane and the distance
between each pair of neighbouring
points row wise or column wise is unity. Assume further that every
neighbouring pair of <tt>1</tt>'s,
row wise, column wise or diagonally is connected by a line segment. Two line segments emerging
from a point, either join together to
form a longer line segment or form an angle of <span class="MATH">45<sup><tt>o</tt></sup></span>, <span class="MATH">90<sup><tt>o</tt></sup></span>

or <span class="MATH">135<sup><tt>o</tt></sup></span>, thus forming right-angled isosceles triangles. The
existence of hidden right-angled isosceles triangles in an array is illustrated
in the figure below.

</p><p>
</p><div align="CENTER">
<!-- MATH
 $\epsfbox{p3258.eps}$
 -->
<img align="BOTTOM" border="0" src="file://KQl4B9jD.png" alt="\epsfbox{p3258.eps}">
</div>

<p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001001000000000000000">
Input</a>&nbsp;</font>
</h2>

<p>
Input consists of multiple test cases.

</p><p>
For each test case the first line gives
three integers: the case number <span class="MATH"><i>k</i></span>, the number of rows <span class="MATH"><i>m</i></span> and the number of
columns <span class="MATH"><i>n</i></span> of the given array. A space appears between two
neighbouring integers.

</p><p>
Each of the next <span class="MATH"><i>m</i></span> lines gives a string
of <tt>0</tt>'s and <tt>1</tt>'s of length <span class="MATH"><i>n</i></span>; the <span class="MATH"><i>i</i></span>-th line gives the <span class="MATH"><i>i</i></span>-th row of the array.


</p><p>
Input terminates with a value zero for case number <span class="MATH"><i>k</i></span>.

</p><p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001002000000000000000">
Output</a>&nbsp;</font>
</h2>

<p>
For each test case, display output in
one line. The line contains the case number <span class="MATH"><i>k</i></span> and the area of the largest
right-angled isosceles triangle hidden in the array. The area is a real number
with one digit after the decimal point. If a triangle does
not exist then output `<tt>0.0</tt>' as the area.


</p><p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001003000000000000000">
Sample Input</a>&nbsp;</font>
</h2>

<p>
</p><pre>1 3 3
101
100
101
2 4 6
001001
010101
111111
000001
0
</pre>

<p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001004000000000000000">
Sample Output</a>&nbsp;</font>

</h2>

<p>
</p><pre>1 0.0
2 4.0
</pre>

<p>
</p><hr><address>Kanpur-Kolkata 2004-2005</address><p>

</p>