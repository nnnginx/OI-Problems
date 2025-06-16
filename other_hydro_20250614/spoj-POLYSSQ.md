<p>You are given N different points in the plane. No any 3 of them are collinear. Write a program that finds out the smallest area of a convex polygon with K vertices which are taken from the given points. 
</p><h3>Input</h3>
<p>Two integers, N and K, are written on the first line in the standard input. It follows N lines, each containing a pair of coordinates for the corresponding given point. Every two numbers on a line in the input are separated by a space. 
Constraints: 0 &lt; N &lt; 50, 0 &lt; K &lt; 11. The coordinates of the given points are nonnegative integers, less than 9999.
</p><h3>Output</h3>
<p>Your program has to output an integer that is equal to the integer part of minimal area. If there does not exist any convex polygon as is described above, your program has to output 0. 

</p><h3>Example</h3>

<pre><b>Input:</b>
4 3
0 0
1 1
0 10
10 0

<b>Output:</b>
5
</pre>