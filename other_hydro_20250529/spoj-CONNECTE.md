<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/CONNECTE/en/">English</a></td>
<td width="50%"><a href="/problems/CONNECTE/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Consider a regular grid of 3 ¡Á N points. Every point in the grid has up to eight neighboring points (see Fig. 1).</p>
<p><img src="../../../SPOJVN/content/CONNECTE1" alt=""></p>
<p>Figure 1: Neighboring points (marked by arrows).</p>
<p>We are interested in counting the number of different ways to connect the points of the grid to form     a polygon that fulfills the following conditions:     1. The set of vertices of the polygon consists of all 3 ¡Á N points.     2. Adjacent vertices of the polygon are neighboring points in the grid.     3. Each polygon is simple, i.e. there must not be any self-intersections.     Two possible polygons for N = 6 are given in the Fig. 2.</p>
<p><img src="../../../SPOJVN/content/CONNECTE2" alt=""></p>
<p>Figure 2: Two possible connections of points for N = 6.</p>
<p>Write a program that calculates for a given N the number of possible ways to connect the points as     described modulo 1,000,000,000.</p>
<h3>Input</h3>
<p>The first and only line contains one positive integer N (N &lt;= 1,000,000,000).</p>
<h3>Output</h3>
<p>The only line to be written contains the remainder of the number of ways to connect the points modulo 1,000,000,000.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3

<strong>Output:</strong>
8

<strong>Input:</strong>
4

<strong>Output:</strong>
40</pre>
<p> </p>