<p align="justify">We say that two triangles intersect if their interiors have at least one common point. A polygon is called convex if every segment connecting any two of its points is contained in this polygon. A triangle whose vertices are also vertices of a convex polygon is called an elementary triangle of this polygon. A triangulation of a convex polygon is a set of elementary triangles of this polygon, such that no two triangles from the set intersect and a union of all triangles covers the polygon. We are given a polygon and its triangulation. What is the maximal number of triangles in this triangulation that can be intersected by an elementary triangle of this polygon?</p>

<h3>Example</h3>
<p align="justify">Consider the following triangulation:</p>
<p align="center"><img src="/content/ahven:wierys.png"></p>
<p align="justify">The elementary triangle (1,3,5) intersects all the triangles in this triangulation.</p>

<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="">
        <li>reads the number of vertices of a polygon and its triangulation; </li>
        <li>computes the maximal number of triangles intersected by an elementary triangle of the given polygon; </li>
        <li>writes the result to standard output.</li>
</ul>
</div>
<h3>Input</h3>
<p align="justify">The number of test cases <i>t</i> is in the first line of input, then <i>t</i> test cases follow separated by an empty line</p>
<p align="justify">In the first line of a test case there is a number <i>n</i>, 3 &lt;= <i>n</i> &lt;= 1000, which equals the number of vertices of the polygon. The vertices of the polygon are numbered from 0 to <i>n</i>-1 clockwise. The following <i>n</i>-2 lines describe the triangles in the triangulation. There are three integers separated by single spaces in the (<i>i</i>+1)-st line, where 1 &lt;= <i>i</i> &lt;= <i>n</i>-2. These are the numbers of the vertices of the <i>i</i>-th triangle in the triangulation. </p>

<h3>Output</h3>
<p align="justify">For each test case your program should produce one line with exactly one integer - the maximal number of triangles in the triangulation, that can be intersected by a single elementary triangle of the input polygon. </p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
6
0 1 2
2 4 3
0 5 4
2 4 0

<b><tt>Sample output:</tt></b>
4
</pre>