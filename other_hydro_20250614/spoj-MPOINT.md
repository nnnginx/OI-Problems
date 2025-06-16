<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MPOINT/en/">English</a></td> 
<td width="50%"><a href="/problems/MPOINT/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<pre>N points are given in a plane. Any point has integer coordinates and no
two points have the same x coordinates or the same y coordinates. 
A pair of points A and B uniquely define a rectangle R(A,B) whose sides
are parallel to coordinate axes such that the points A and B are endpoints
of one of its diagonals. A pair of two given points A and B are  very visible 
if there are  no other given points within a rectangle R(A,B). A pair of points 
consists of two different points and in this problem pairs (A,B) and (B,A)
are regarded to be the same pair and are counted as one pair. 

At the beginning a coordinate plane has no given points. Your program should read 
coordinates of the given points and after reading coordinates of a point, 
it should write number of pairs of currently very visible given points.  
</pre>
<h3>Input</h3>
<pre>First line of input contains an integer N, 2 ¡Ü N ¡Ü 5000, the number of given 
points. 
Each of the following N lines contains two integers X, Y, 0  ¡Ü X,Y  ¡Ü 10^6, 
coordinates of the given points in the order they should be added to the plane.
</pre>
<h3>Output</h3>
<pre>An output should contain N lines, kth  line should contain a number 
of pairs of very visible given points after taking kth
given point into account. 
</pre>
<h3>Sample</h3>
<pre>input 
 
7 
1 5 
2 7 
3 8 
5 1 
6 2 
7 3 
4 4 
 
output 
 
0 
1 
2 
5 
9 
13 
10 

input 
 
4 
2 3 
3 4 
1 2 
4 1 
 
output 
 
0 
1 
2 
5 
 </pre>