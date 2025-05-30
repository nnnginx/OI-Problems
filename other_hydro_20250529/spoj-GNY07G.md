<p>Just when you thought we had run out of model rocket height problems...
</p><p>Yet another method used to determine the height achieved by a model rocket is the vertical line
method. Two observers A and B are spaced D feet apart along a base line along one edge of the flat
test field. The launch platform is equidistant from observers A and B and L feet from the base line.
Each observer has a theodolite or some other device for measuring angle above the horizontal
(elevation angle) of a distant object and the azimuth angle (the angle the vertical plane of the sight
line makes with the line from A through B measured counter-clockwise). Each measuring device is on
a stand. A��s device is HA feet above the level of the launch platform and B��s device is HB feet above
the level of the launch platform. When a rocket is fired, near the top of its flight, it deploys a parachute
and emits a puff of smoke. Each observer measures the elevation angle and azimuth angle of the puff
of smoke from their location. If the peak location is on the wrong side of the baseline or outside the
lines determined by A and B perpendicular to the base line, it is out of bounds and disqualified. From
this information, the height of the rocket may be determined as follows:
</p><p>Each sight line determines a vertical plane. These two planes intersect in a vertical line (thus the
name of the method). Each sight line intersects this vertical line in a point. If these points are more
than ERRDIST feet apart, an error is assumed and the flight is rejected. Otherwise, the point halfway
between the two points where a sight line intersects the vertical line is computed. The rocket height is
the distance of this midpoint above the launch platform.
</p><p>You must write a program which, given the parameters D (the distance in feet between observers A
and B), L (the distance in feet from the base line to the launch platform), HA (the distance of the
measuring device A above the launch platform in feet), HB (the distance of the measuring device B
above the launch platform in feet), ERRDIST (the maximum distance between the intersection points
of a sight line with the vertical line), �� (the elevation angle of the rocket in degrees measured by the
left observer A), �� (the elevation angle of the rocket in degrees observed by the right observer B), ��
(the azimuth angle in degrees measured by the left observer A) and �� (the azimuth angle in degrees
measured by the right observer B), computes the height of the rocket above the launch platform in
feet to the nearest foot.

</p><h3>Input</h3>
<p>The first line of input contains a single integer N, (1 �� N �� 1000) which is the number of datasets that
follow.
</p><p>The second line contains the parameters D, L, HA, HB and ERRDIST in that order as (floating point)
decimal values. These values would be measured once at the beginning of the day and remain fixed
through all rocket shots.
</p><p>Each succeeding line of input represents a single dataset. Each dataset will contain the angles ��, ��,
�� and �� in that order (measured in degrees) as (floating point) decimal values for a rocket shot.

</p><h3>Output</h3>
<p>For each dataset of four angles, the output consists of a single line . If angles ��, �� and �� are not
strictly between 0 and 90 degrees or �� is not strictly between 90 degrees and 180 degrees, the line
should contain the dataset number, a space and the word ��DISQUALIFIED�� (without the quotes).
Otherwise, if the distance between the intersection points of a sight line with the vertical line is more
that ERRDIST feet, the line should contain the dataset number, a space and the word ��ERROR��
(without the quotes). Otherwise, the line should contain the dataset number, a space and the height
above the launch platform in feet to the nearest foot.

</p><h3>Example</h3>

<pre><b>Input:</b>
4
100.0 300.0 5.25 2.92 5.00
40.1 36.2 35.3 151.6
64.9 71.1 15.7 160.1
44.9 41.2 33.1 152.5
44.9 41.2 33.1 52.5

<b>Output:</b>
1 50
2 ERROR
3 58
4 DISQUALIFIED
</pre>