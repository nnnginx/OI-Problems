<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Aang is fond of geometric figures, especially with equilateral triangles. He likes to know how well equilateral triangles cooperate with other figures.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">He initially takes an equilateral triangle of side t1. He also takes a square of side a, rectangle of dimensions l and b, another equilateral triangle of side t2&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">and a circle of radius r. He then takes turn and places each figure near the initial equilateral triangle of side t1. While placing nearer, he can place those&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">figures in any orientation, any two edges of the two figures can be along same line but the figures cannot overlap. He now needs to find a cooperation value&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">which is the minimum area of the rectangle needed to surround the area of the two figures. For example, when he places a square near a triangle, the cooperation&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">value is the area of the smallest rectangle which can surround the areas of the triangle and square. Now, given the values, find the cooperation values of all&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">the figures with the initial equilateral triangle.</div>
<p>Aang is fond of geometric figures, especially with equilateral triangles. He likes to know how well equilateral triangles cooperate with other figures. He initially takes an equilateral triangle of side t1. He also takes a square of side a, rectangle of dimensions l and b, another equilateral triangle of side t2 and a circle of radius r. He then takes turn and places each figure near the initial equilateral triangle of side t1. While placing nearer, he can place those figures in any orientation, any two edges of the two figures can be along same line but the figures cannot overlap. He now needs to find a cooperation value which is the minimum area of the rectangle needed to surround the area of the two figures. For example, when he places a square near a triangle, the cooperation value is the area of the smallest rectangle which can surround the areas of the triangle and square. Now, given the values, find the cooperation values of all the figures with the initial equilateral triangle.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line consists of t, the number of test cases (1 &lt;= t &lt;= 20)</p>
<p>Next t lines consists of 6 values t1, a, l, b, t2 and r denoting side of first triangle, side of square, length and breadth of rectangle, side of second triangle and radius of circle. (all values will lie between 1 and 100 inclusive)</p>
<p><strong><span style="font-size: 1.17em;">Output</span></strong></p>
<p>For each test case, print a single line consisting of the cooperation values of the first triangle with the square, rectangle, circle and the other triangle respectively. (separated by spaces rounded off to 4 decimal digits)</p>
<p><strong><span style="font-size: 1.17em;">Example</span></strong></p>
<pre><strong>Input:</strong>
1
2 2 2 3 2 1

<strong>Output:</strong>
7.4641 9.4641 7.4641 5.1962</pre>