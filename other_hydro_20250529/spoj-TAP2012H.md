<p><span style="font-style: italic;">[The original version of this problem (in Spanish) can be found at&nbsp;</span><a style="font-style: italic;" href="http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf</a><span style="font-style: italic;">]</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">To go on holidays, Horacio and Hernan have sacrificed their participation in an important programming contest. While you are in this contest, they are close to the Andes driving along Highway 40, in Argentina, enjoying a pleasant view of the mountains in the horizon. Right now the sky over the highway is a clear, uniform blue, while the visible part of the mountains is a profile presenting rich and attractive textures. This worries Horacio and Hernan, because they fear that the pictures they are taking will be very expensive to print correctly. For this reason, in the next stop they will take out their laptops and write a program to estimate the area of the mountain profile that has to be printed in each picture. Can you finish this program before them?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Horacio and Hernan will be modeling the mountain profile in the following way. Each mountain is represented by an isosceles triangle whose base rests on the X axis of the XY plane. Two equal-length sides connect the endpoints of the base to the opposite vertex of the triangle, which is the tip of the corresponding mountain. To describe the position and shape of the triangle, we use the coordinates along the X axis of the base endpoints, along with the height of the mountain.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">
<p>The figure below is the model of a mountain profile formed by 4 mountains that are overlapping with one another. The area of the surface of the mountain profile that you have to calculate is marked with stripes. The lowest mountain of the figure is described by the values I = 4 (the left endpoint of the mountain base), D = 5 (the right endpoint of the mountain base) &nbsp;and H = 1 (the height of the</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>mountain)</p>
</div>
<p>To go on holidays, Horacio and Hernan have sacrificed their participation in an important programming contest. While you are in this contest, they are close to the Andes driving along <em>Highway 40</em>, in Argentina, enjoying a pleasant view of the mountains in the horizon. Right now the sky over the highway is a clear, uniform blue, while the visible part of the mountains is a profile presenting rich and attractive textures. This worries Horacio and Hernan, because they fear that the pictures they are taking will be very expensive to print correctly. For this reason, in the next stop they will take out their laptops and write a program to estimate the area of the mountain profile that has to be printed in each picture. Can you finish this program before them?</p>
<p>Horacio and Hernan will be modeling the mountain profile in the following way. Each mountain is represented by an isosceles triangle whose base rests on the <strong>X</strong> axis of the <strong>XY</strong> plane. Two equal-length sides connect the endpoints of the base to the opposite vertex of the triangle, which is the tip of the corresponding mountain. To describe the position and shape of the triangle, we use the coordinates along the <strong>X</strong> axis of the base's endpoints, along with the height of the mountain.</p>
<p>The figure below is the model of a mountain profile formed by <strong>4</strong> mountains that are overlapping with one another. The area of the mountain profile that you have to calculate is marked with stripes. The lowest mountain of the figure is described by the values <strong>I = 4</strong> (the left endpoint of the mountain base), <strong>D = 5</strong> (the right endpoint of the mountain base) &nbsp;and <strong>H = 1</strong> (the height of the mountain).</p>
<p style="text-align: center;"><img title="TAP2012H" src="/content/fidels:TAP2012H.png" alt="TAP2012H"></p>
<p>In this problem, you are given the representation of the mountain profile, and you have to find the area of the union of all the corresponding triangles, in such a way that the overlapping parts are counted only once.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Each test case is described using several lines. The first line contains a single integer number <strong>N</strong>, indicating the number of mountains (<strong>1 ¡Ü&nbsp;N&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;1000</strong>). Each of the <strong>N</strong> following lines describes a mountain using three integer numbers <strong>I</strong>, <strong>D</strong> and <strong>H</strong>, representing respectively the <strong>X</strong> coordinate of the left endpoint of the base, the same for the right endpoint of the base, and the height of the mountain (<strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;I, D, H&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;10<sup>5</sup></strong> with <strong>I &lt; D</strong>). In each test case there are no two mountains that are exactly the same (that is, with equal values for the three parameters <strong>I</strong>, <strong>D</strong> and <strong>H</strong>). The end of the input is signalled by a line containing the number <strong>-1</strong>.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, you should print a single line containing a rational number, representing the area of the corresponding mountain profile. Round the result to the closest rational with two decimal digits. In case of ties, round up. Note that you should always use exactly two digits after the decimal dot, even if this means ending with a zero.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">4
4 5 1
2 4 2
3 5 3
3 7 2
1
1 2 1
2
10 20 20
20 40 10
2
15 25 20
20 40 10
7
99998 99999 25000
99998 100000 50000
99996 100000 100000
1 3 100000
2 5 100000
1 5 60000
1 99999 100000
5
2 3 10
4 5 6
6 8 11
12 14 3
1 13 2
-1</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">6.90
0.50
200.00
190.00
5000331093.88
28.91</span><span style="white-space: normal;">
</span></pre>