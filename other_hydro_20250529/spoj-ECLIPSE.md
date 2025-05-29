<p>Every so often we hear on the news that there is going to be either a solar or lunar eclipse. Eclipses
have a long history dating back well into the BC’s. Astronomers study total solar eclipses very closely
as they provide the rare opportunity to observe the corona.
</p><p>An eclipse occurs when two celestial bodies and a star are (nearly) linearly aligned and the shadow
cast by the one body intersects the other body, creating darkness on the latter body.
</p><p>We are interested in determining when a solar eclipse will next occur. In Figure 1 you can see two
labelled regions. The umbra is the area of total darkness — a body in this region will experience a total
solar eclipse. The penumbra is the area of partial darkness — a body in this region will experience a
partial solar eclipse.
</p><p>You will be given the size and location of a star and two celestial bodies. Your task is to determine if
the first celestial body creates a solar eclipse on the second celestial body. If it does then you are to
determine whether it is a total or partial eclipse and whether the entire body is in eclipse. If part of
the body is experiencing total eclipse while the entire body is experiencing at least a partial eclipse,
we are only interested in the part that is in total eclipse.
</p><p>Consider a scaled model of our solar system with the sun at the origin (0, 0, 0) with radius 700, the
moon at position (49900, 1000, 149700) with radius 2 and Earth at position (50000, 1000, 150000) with
radius 7. In Figure 1, the sun would be the star on the left and the moon would be the smaller body
on the right. Part of Earth would then fall in the black umbra region and hence partly experience a
total solar eclipse.
</p><p>For any body:
</p><li> 1 ≤ r ≤ 10<sup>6</sup>
</li><li> 0 ≤ x, y, z ≤ 10<sup>9</sup>
<p>It is guaranteed that any two bodies will be at least 1
unit apart, and that moving any one of the bodies by 1
unit (in any direction) will not change the answer.</p>
<p><img src="/content/marcog:eclipse.png">

</p><h3>Input</h3>
<p>A test case is described by three lines, each describing the size and location of a single body. The
first line contains four space-separated integers xs , ys , zs and rs , describing the center (xs , ys , zs ) and
radius rs of the star. The following two lines define the two celestial bodies in the same manner.
</p><p>Test cases follow directly after one another with a −1 representing the end of the test cases.

</p><h3>Output</h3>
<p>Each test case has a single line of output describing the type of eclipse for that case. If the second
celestial body listed in the test case is experiencing an eclipse, then one of the following lines must be
output:
</p></li><li>Entire total solar eclipse
</li><li>Part total solar eclipse
</li><li>Entire partial solar eclipse
</li><li>Part partial solar eclipse
<p>If there is no solar eclipse, the line “No solar eclipse” must be output.

</p><h3>Example</h3>

<pre><b>Input:</b>
0 0 0 700
49900 1000 149700 2
50000 1000 150000 7
0 0 0 10
50 0 100 40
60 0 200 1
-1

<b>Output:</b>
Part total solar eclipse
Entire total solar eclipse</pre>
</li>