<p>R2D2 was exploring a tunnel when a cave-in suddenly occurred. Oh no, is he trapped?</p>
<p>&nbsp;</p>
<div><img src="../../../content/min_25:pc8c.png" border="0" alt="epsfbox{p4434.eps}" width="640" align="BOTTOM"></div>
<p>&nbsp;</p>
<div>Figure1: Overhead view of the cave crisis from the third example test case.</div>
<p>From an overhead view, we can see all the obstacles (debris) on a two-dimensional Cartesian plane. The tunnel is <span><em>w</em></span> cm wide, bounded by the lines <span><em>y</em> = <em>w</em>/2</span> and <span><em>y</em> = - <em>w</em>/2</span>. R2D2 starts at <span>(0, 0)</span>, and has a perfectly circular footprint of radius <span><em>r</em></span>. The exit of the tunnel lies to the right of the line <span><em>x</em> = 1000</span>. Between R2D2 and the exit lie a number of polygonal obstacles.</p>
<p>Is it possible for R2D2 to navigate between the obstacles and make it to the exit?</p>
<h3>Input</h3>
<p>The input file will contain multiple test cases. Each test case begins with a single line containing an even  integer <span><em>w</em></span> ( <span>2 ¡Ü <em>w</em> ¡Ü 1000</span>), the width of the tunnel, and an integer <span><em>N</em></span> ( <span>0 ¡Ü <em>N</em> ¡Ü 100</span>), the number  of obstacles. The next <span><em>N</em></span> lines each contain the description of a single obstacle. The <span><em>i</em></span>-th obstacle is a simple  polygon, specified on a single line containing an integer <span><em>n</em><sub>i</sub></span> ( <span>3 ¡Ü <em>n</em><sub>i</sub> ¡Ü 10</span>), the number of vertices, followed  by <span><em>n</em><sub>i</sub></span> pairs of integers, <span><em>x</em><sub>ij</sub></span> and <span><em>y</em><sub>ij</sub></span> ( <span>0 ¡Ü <em>x</em><sub>ij</sub> ¡Ü 1000</span> and  <span>-<em>w</em>/2 ¡Ü <em>y</em><sub>ij</sub> ¡Ü <em>w</em>/2</span> for   <span><em>j</em> = 1,..., <em>n<sub>i</sub></em></span>), specifying the  coordinates of the vertices in counterclockwise order. Note that  obstacles in the input may touch or even overlap. However, you are  guaranteed that R2D2's initial location will not touch or overlap any  obstacle. The vertices of each polygon are unique, no two nonconsecutive  edges of the polygon intersect (even at their endpoints), and each  polygon is guaranteed to have nonzero area.</p>
<p>The end-of-input is denoted by an invalid test case with <span><em>w</em> = <em>N</em> = 0</span> and should not be processed.</p>
<h3>Output</h3>
<p>For each input test case, you must determine the maximum radius <span><em>r</em> &gt; 0</span> that R2D2 could have and still be able to plan a path from his starting location <span>(0, 0)</span> to the tunnel exit without overlapping with any of the obstacles. You should print either this maximum radius <span><em>r</em></span> (rounded to two decimal places) or the message "<tt>impossible</tt>" if no such radius exists.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>&nbsp;<pre>6 2
4 2 -1 4 -1 4 1 2 1
3 3 0 6 -1 6 1
8 2
3 1 -1 4 -1 4 4
3 3 -4 6 1 3 1
10 7
4 0 5 4 2 5 3 4 5
3 4 -5 9 -5 9 0
4 8 -5 11 -5 11 -2 8 -2
3 8 3 16 1 11 5
4 21 -5 23 -3 20 -2 15 -4
3 22 3 26 -1 28 0
3 24 0 29 4 25 3
0 0</pre>
<strong>Output:</strong>&nbsp;
<pre>1.00
impossible
1.33
</pre>
</pre>