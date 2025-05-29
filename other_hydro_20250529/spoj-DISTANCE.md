<p>The L<sub>1</sub> distance of two d-dimensional points is the sum of
absolute values of their coordinate differences (i.e.
¦²<sub>i=1</sub><sup>d</sup> |x<sub>i</sub> - y<sub>i</sub>| for two points x,y).  Given N points in
the plane you must find the farthest pair of points under the L<sub>1</sub>
distance metric and output their distance.

</p><h3>Input</h3>
<p>The first line of the input is "N d" (2 ¡Ü N ¡Ü 100000, 1 ¡Ü
d ¡Ü 6) signifying that there are N points in d-dimensional
space.  N lines then follow, where the ith line is a
space-separated list of d numbers, the coordinates of the ith point.
All given coordinates are integers that are at most 1000000 in
absolute value, and all given points are distinct.

</p><h3>Output</h3>
<p>Your output should consist of a single integer, the farthest distance
between a pair of input points, followed by a newline.

</p><h3>Example</h3>

<pre><b>Input:</b>
3 2
0 0
-5 0
1 1

<b>Output:</b>
7
</pre>