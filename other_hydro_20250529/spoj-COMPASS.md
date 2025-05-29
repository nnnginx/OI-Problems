<p>A group of adventurers are on an expedition to reach the North Pole. The only instrument they have is a compass that points to the pole.
However, the compass is broken and although its measurements are consistent, the direction it points to is some fixed but unknown angle away from true North. For example, if the error angle is 90 degrees, the compass will always point East at times when it should point North. This error angle may be zero, in which case the compass is not broken.

</p><h3>Input</h3>
<p>To overcome this difficulty the group decided to take measurements at several different points and try to recover the location of the North pole from that. For simplicity, we assume that the region around the North pole is a plane in which a coordinate system is introduced.
Each point is then described by a pair of real numbers (x,y), x,y ¡Ê [-200, 200]. One of those points (not necessarily (0,0)) is the location of the pole. The compass would always point to that location if it were not broken. Instead, it always points a fixed angle away from the true direction to the pole.

In this problem we assume that the magnetic pole is the same as the geographic pole and that it is a point source.

</p><h3>Output</h3>
<p>The first line of input specifies one integer number N, N &lt; 10, the number of measurements taken. Each of the next N lines contains four space separated real numbers: the first two are the x and y coordinates of the point at which the measurement was taken, the third and fourth are (u<sub>x</sub>, u<sub>y</sub>), the direction of a unit vector indicating where the compass needle points. 

There should be only one line of output that should contain two real numbers separated by space: the x and y coordinates of the pole. Your output is considered correct if it is within an additive 0.01 of the correct answer.

All measurements are consistent and it is always possible to determine the location of the North pole from them. None of the measurements is made on the pole.

</p><h3>Example</h3>

<pre><b>Input:</b>
4
1.000000 0.000000 -0.000000 -1.000000
-1.000000 0.000000 0.000000 1.000000
0.000000 1.000000 1.000000 0.000000
0.000000 -1.000000 -1.000000 0.000000

<b>Output:</b>
0.000000 0.000000
</pre>