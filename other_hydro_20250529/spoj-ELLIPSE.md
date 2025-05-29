<p>Given 5 points on a ellipse, calculate the area of the ellipse. We accept solutions with <b>absolute error less than 10<sup>-6</sup> or relative error less than 10<sup>-9</sup></b>.</p>
<h3>Input</h3>
<p>Many test cases. Each contains a line with 10 integers with absolute value less than 1000 - the X and Y coordinates of the 5 points, respectively.
</p><p>Input terminates by EOF. Note that there can be extra spaces in a single line.</p>
<h3>Output</h3>
<p>Each line contains a single float-point number - the area of the corresponding ellipse, or "IMPOSSIBLE" if the ellipse doesn't exist or can't be unique determined.</p>
<h3>Example</h3>
<pre><b>Input:</b>
6 1 3 2 -2 -3 -3 -2 1 6
7 -3 2 7 6 3 5 5 -2 -9

<b>Output:</b>
IMPOSSIBLE
157.079633
</pre>
<p><b>Note: You can click on "Wrong Answer" to get further information.</b>
</p><p><b>Note: Judge is slightly modified to avoid some precision problems. </b></p>