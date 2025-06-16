## Description

<div><p>A point <span class="tex-font-style-it">belongs</span> to a triangle if it lies inside the triangle or on one of its sides. Two triangles are <span class="tex-font-style-it">disjoint</span> if there is no point on the plane that belongs to both triangles.</p><p>You are given $n$ points on the plane. No two points coincide and no three points are collinear.</p><p>Find the number of different ways to choose two disjoint triangles with vertices in the given points. Two ways which differ only in order of triangles or in order of vertices inside triangles are considered equal.</p></div><div class="input-specification"><p>The first line of the input contains an integer $n$ ($6 \le n \le 2000$) 每 the number of points.</p><p>Each of the next $n$ lines contains two integers $x_i$ and $y_i$ ($|x_i|, |y_i| \le 10^9$) 每 the coordinates of a point.</p><p>No two points coincide and no three points are collinear.</p></div><div class="output-specification"><p>Print one integer 每 the number of ways to choose two disjoint triangles.</p></div>

## Input

<p>The first line of the input contains an integer $n$ ($6 \le n \le 2000$) 每 the number of points.</p><p>Each of the next $n$ lines contains two integers $x_i$ and $y_i$ ($|x_i|, |y_i| \le 10^9$) 每 the coordinates of a point.</p><p>No two points coincide and no three points are collinear.</p>

## Output

<p>Print one integer 每 the number of ways to choose two disjoint triangles.</p>

## Samples

```input1
6
1 1
2 2
4 6
4 5
7 2
5 3

```

```output1
6

```






```input2
7
0 -1000000000
-5 -5
5 -5
-5 0
5 0
-2 2
2 2

```

```output2
21

```




## Note

<p>In the first example there are six pairs of disjoint triangles, they are shown on the picture below.</p><center> <img class="tex-graphics" height="302px" src="./29486/file/uZ4egYEN.png" style="max-width: 100.0%;max-height: 100.0%;" width="529px"> </center><p>All other pairs of triangles are not disjoint, for example the following pair:</p><center> <img class="tex-graphics" height="124px" src="./29486/file/UdL38Miz.png" style="max-width: 100.0%;max-height: 100.0%;" width="147px"> </center>
