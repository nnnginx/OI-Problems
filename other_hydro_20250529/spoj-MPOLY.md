<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MPOLY/en/">English</a></td> 
<td width="50%"><a href="/problems/MPOLY/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p></p><p>
There are N points in a plane whose coordinates are natural numbers.
A convex polygon with maximal number of vertices is a convex polygon 
whose vertices are some of given points and the origin having maximal 
possible number of vertices. Origin, i.e. point with coordinates 
(0,0), must be one of vertices of a convex polygon with maximal number
of vertices.</p><p>
Write a program that will determine number of vertices in such polygon.</p><p>
A polygon is convex if every line segment whose endpoints are inside 
that polygon is also completely inside it.
Consecutive edges of a polygon must not be parallel.</p><p>

 

</p><h3>Input</h3>
<p></p><p>
The first line of input file contains a natural number N, 2 ¡Ü N ¡Ü 100, 
a number of given points.</p><p>
Each of the following N lines contains two natural numbers X and Y, 
1 ¡Ü X ¡Ü 100, 1 ¡Ü Y ¡Ü 100, separated by a space character, coordinates of 
one point. </p><p>All points will be different.</p><p>


 
</p><h3>Output</h3>
<p></p><p>
The first and only line of output file should contain number of vertices
of convex polygon with maximal number of vertices.
Note: the result will always be at least 3.</p><p>


</p><h3>Sample</h3>
<pre>POLYGON.IN

5
4 2
2 2
2 3
3 2
3 1

POLYGON.OUT

4
 
POLYGON.IN

8
10 8
3 9
2 8
2 3
9 2
9 10
10 3
8 10

POLYGON.OUT

8
 
POLYGON.IN

10
9 6
1 7
2 2
3 9
8 7
3 2
9 4
3 1
9 7
6 9

POLYGON.OUT

7
Explanation for test data #2 (coordinates of polygon)

2 8
3 9
8 10
9 10
10 8
10 3
9 2
0 0

</pre>