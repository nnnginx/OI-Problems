<p align="justify">
At the beginning of spring all the sheep move to the higher pastures in the mountains. If there are thousands of them, it is well worthwhile gathering them together in one place. But sheep don't like to leave their grass-lands. Help the shepherd and build him a fence which would surround all the sheep. The fence should have the smallest possible length! Assume that sheep are negligibly small and that they are not moving. Sometimes a few sheep are standing in the same place. If there is only one sheep, it is probably dying, so no fence is needed at all...
</p>
<h3>Input</h3>
<p align="justify">
<br>t [the number of tests &lt;= 100]
<br>[empty line]
<br>n [the number of sheep &lt;= 100000]
<br><i>x</i><sub>1</sub> <i>y</i><sub>1</sub> [coordinates of the first sheep]
<br>...
<br><i>x<sub>n</sub></i> <i>y<sub>n</sub></i>
<br>[integer coordinates from -10000 to 
10000]
<br>[empty line]
<br>[other lists of sheep]
<br>
<br>
Text grouped in [ ] does not appear in the input file. Assume that sheep are numbered in the input order.
</p>
<h3>Output</h3>
<p align="justify">
<br>o [length of circumference, rounded to 2 decimal places]
<br>p1 p2 ... pk 
<br>[the sheep that are standing in the corners of the fence; the first one should be positioned bottommost and as far to the left as possible, the others ought to be written in anticlockwise order; ignore all sheep standing in the same place but the first to appear in the input file; the number of sheep should be the smallest possible]
<br>[empty line]
<br>[next solutions]
</p>
<h3>Example</h3>
<pre>Input:
8

5
0 0
0 5
10 5
3 3
10 0

1
0 0

3
0 0
1 0
2 0

4
0 0
0 0
0 1
1 0

3
0 0
0 1
1 0

6
0 0
-1 -1
1 1
2 2
3 3
4 4

2
10 0
0 0

7
-3 -4
2 -3
4 3
-4 2
0 5
2 -3
-1 4

Output:
30.00
1 5 3 2

0.00
1

4.00
1 3

3.41
1 4 3

3.41
1 3 2

14.14
2 6

20.00
2 1

26.98
1 2 3 5 4

</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>