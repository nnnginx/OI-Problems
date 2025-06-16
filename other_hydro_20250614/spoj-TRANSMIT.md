<p>
In a wireless network with multiple transmitters sending on the same
frequencies, it
is often a requirement that signals don't overlap, or at least that they don't
conflict. One way of accomplishing this is to restrict a transmitter's coverage
area. This problem uses a shielded transmitter that 
only broadcasts in a semicircle.
</p>
<p>
A transmitter <i>T</i> is located somewhere on a 1,000 square meter grid.
It broadcasts in a semicircular area of radius <i>r</i>. The
transmitter may be rotated any amount, but not moved. 
Given <i>N</i> points anywhere on the grid, compute
the maximum number of points that can be simultaneously reached by the
transmitter's signal.
Figure 1 shows the
same data points with two different transmitter rotations.

</p>

<center><img src="./24722/file/8MhepRe7.png"></center>

<p>
All input coordinates are integers (0-1000). The radius is a
positive real number greater than 0.
Points on the boundary of a semicircle are considered within that
semicircle.  There are 1-150 unique points to examine per transmitter.
No points are at the same location as the transmitter.
</p>

<p>
Input consists of information for one or more independent transmitter problems.
Each problem begins with
one line containing the (x,y) coordinates of the transmitter followed by the
broadcast radius, <i>r</i>.
The next line contains the number of points <i>N</i> on the grid,
followed by <i>N</i> sets of (x,y) coordinates, one
set per line.  The end of the input is signalled by a line with a
negative radius; the (x,y) values will be present but indeterminate.
Figures 1 and 2 represent the data in the first two example data sets below,
though they are on different scales. Figures 1a and 2 show
transmitter rotations that result in maximal coverage.

</p>

<p>For each transmitter, the output contains a single line with 
the maximum number of points that can be contained in some semicircle.
</p>

<pre><b>Input:</b>
25 25 3.5
7
25 28
23 27
27 27
24 23
26 23
24 29
26 29
350 200 2.0
5
350 202
350 199
350 198
348 200
352 200
995 995 10.0
4
1000 1000
999 998
990 992
1000 999
100 100 -2.5
</pre>


<pre><b>Output:</b>
3
4
4
</pre>