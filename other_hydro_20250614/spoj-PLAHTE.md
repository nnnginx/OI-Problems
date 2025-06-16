<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/PLAHTE/en/">English</a></td> 
<td width="50%"><a href="/problems/PLAHTE/vn/">Vietnamese</a></td> 
</tr></tbody></table>



<p>Mirko washed his sheets and is on his way to hang them to dry in front of his house. However, strong
winds have pulled the clothesline out of the ground so Mirko temporarily laid out the sheets on the
grass.</p>
<p>The grass field can be modeled by an infinite square grid, where every unit square is represented by a
pair of coordinates. Sheets are rectangles in the grid with sides parallel to the coordinate axes. Sheets
may overlap.</p>
<p>In an effort to put his clothesline back up, Mirko slammed a pole into the ground at coordinates (0, 0).
An entirely unexpected turn of events followed. Oil sprung from the ground and the shock caused
Mirko to faint. While Mirko lay unconscious, the oil is spreading, staining his sheets.</p>
<p>Time is measured from the moment the oil starts spreading – at time zero only square (0, 0) is covered
in oil. The oil is spreading at a speed of one square per second in all eight directions, as shown in
the figure below. When oil enters a square, it stains that square of fabric on all sheets covering the
square.</p>

<img src="./23875/file/Hx5GyGPY.png">

<p>Write a program that, given M points in time, calculates the total area of stained fabric on all sheets
for each of the given time points.</p>

<h3>Input</h3>
<p>The first line contains an integer N (1 ≤ N ≤ 100 000), the number of sheets.</p>
<p>Each of the following N lines contains four integers x1, y1, x2 and y2 (−1 000 000 ≤ x1 ≤ x2 ≤ 1 000 000),
(−1 000 000 ≤ y1 ≤ y2 ≤ 1 000 000). The coordinates (x1, y1) and (x2, y2) represent diagonally opposite
corners of a sheet (again, these coordinates are unit squares, not points on the plane). None of the
sheets will cover the square (0, 0).</p>
<p>The next line contains an integer M (1 ≤ M ≤ 100 000), the number of points in time.</p>
<p>The next line contains M integers between 0 and 1 000 000, the time points. They will be given in
strictly ascending order.</p>

<h3>Output</h3>
<p>For each of the time points, output on a separate line the total area of stained fabric on all sheets, in the
order the time points are given in the input.
</p>
<h3>Example</h3>

<pre><b>Input:</b>
3
-2 1 1 2
1 0 2 1
-3 -3 -2 0
2
1 2

<b>Output:</b>
5
15

<b>Input:</b>
4
5 1 8 4
-8 1 -5 4
-10 2 10 3
6 0 8 10
6
1 2 3 4 7 9

<b>Output:</b>
0
5
14
18
70
100


<b>Input:</b>
1
1 1 1000000 1000000
3
100 10000 1000000

<b>Output:</b>
10000
100000000
1000000000000

</pre>