<p align="justify">The GX Light Pipeline Inc. started to prepare bent pipes for the new transgalactic light pipeline. However during the design of the pipeline they ran into the problem of determing how far the light can reach inside the pipe. In order to improve your scarce budget you decided to fill a summer job at the GX Light Pipeline Inc. Now it's your task to create a program which computes how far the light reaches in the pipeline.</p>
<p align="justify">The pipeline consists of seamlessly welded together segments made of non-reflecting opaque materials. The upper points of the pipe contour are described by a sequence of points [<i>x</i><sub>1</sub>, <i>y</i><sub>1</sub>], [<i>x</i><sub>2</sub>, <i>y</i><sub>2</sub>], [<i>x</i><sub>3</sub>, <i>y</i><sub>3</sub>], ..., [<i>x<sub>n</sub></i>, <i>y<sub>n</sub></i>], where <i>x<sub>k</sub></i> &lt; <i>x<sub>k</sub></i><sub>+1</sub>. The bottom points of the pipe contour are the same points with <i>y</i>-coordinate decreased by 1.</p>
<p align="justify">The company wants to find the points with maximal <i>x</i>-coordinate that the light will reach. The light is emitted by a segment source with endpoints [<i>x</i><sub>1</sub>, <i>y</i><sub>1</sub>] and [<i>x</i><sub>1</sub>, <i>y</i><sub>1</sub>-1] (endpoints are emitting light too). Assume that the light is not bent at the pipe bent points and the bent points do not stop the light beam.</p>
<img src="/content/ahven:pipe.gif" align="center">
<h3>Input</h3>
<p align="justify">Each test case starts with the number of bent points <i>n</i>. Each of the next <i>n</i> lines contains a pair of real values <i>x<sub>i</sub></i>, <i>y<sub>i</sub></i> separated by space.</p>
<p align="justify">The number of bent points never excedes 200.</p>
<p align="justify">There are many test cases. Input terminates with <i>n</i> = 0.</p>

<h3>Output</h3>
<p align="justify">For each test case your program should output on a single line the maximal <i>x</i>-coordinate of the point where the light can reach from the source segment, written with precision of two decimal places. If the light goes trough all the pipe, your program should output <i>x<sub>n</sub></i>.</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
4
0.00 1.00
2.00 2.00
4.00 1.00
6.00 4.00
0

<b><tt>Sample output:</tt></b>
4.67
</pre>