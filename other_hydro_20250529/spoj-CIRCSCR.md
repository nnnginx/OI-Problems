<p>Yesterday Andrew wrote a program that draws n white circles on a black screen. The screen is monochrome and it has a resolution w x h pixels. Pixels are numbered from upper left corner (0, 0) to bottom right one (w-1, h-1).</p>
<p>A circle with the center at pixel (x<sub>c</sub>, y<sub>c</sub>) and the radius r consists of the pixels with coordinates (x, y) such that (x<sub>c</sub>-x)<sup>2</sup> + (y<sub>c</sub>-y)<sup>2</sup> &lt;= r<sup>2</sup> . If the circle does not fit on the screen, it is truncated. If some pixel belongs to two or more circles, it is white.</p>
<p style="text-align: center;"><img title="Example" src="../../content/fidels:CIRCLES.png" alt="Example"></p>
<p>The resulting picture was very nice, so Andrew decided to copy it to his wall. He has white wallpaper and he can only draw some parts of wall into black. Now he wants to know the amount of paint he needs.</p>
<p>He copies the picture exactly pixel-to-pixel, so you should write a program that calculates the number of black pixels left on a screen after drawing n circles.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>In the first line of input file there is an integer T, the number of test cases. T test cases follow.</p>
<p>Each test case begins with a line where there are three integers: w, h, and n (1 &lt;= w, h &lt;= 20.000; 1 &lt;= n &lt;= 100). Each of the following n lines contains descriptions of the circles. In i+1-th line there are three integers: x<sub>i</sub>, y<sub>i</sub>, r<sub>i</sub> (0 &lt;= x<sub>i</sub> &lt; w; 0 &lt;= y<sub>i</sub> &lt; h; 0 &lt;= r<sub>i</sub> &lt;= 40 000). They denote a circle with the center at pixel (x<sub>i</sub>, y<sub>i</sub>) and radius r<sub>i</sub>.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case you should output exactly one number - the number of black pixels left on the screen.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
5 3 2
1 1 1
3 1 1
12 9 2
3 3 2
7 5 4

<strong>Output:</strong>
6
51</pre>
<p><span style="white-space: normal;">Note: The picture corresponds to the second test case of the example.</span></p>