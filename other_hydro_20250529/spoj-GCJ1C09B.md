<p><strong>Problem</strong></p>
<p>You are studying a swarm of <strong>N</strong> fireflies. Each firefly is moving  in a straight line at a constant speed. You are standing at the center  of the universe, at position (0, 0, 0). Each firefly has the same mass, and you want to know how close the center of the swarm will get to your location (the origin).</p>
<p>You know the position and velocity of each firefly at t = 0, and are only interested in t �� 0.   The fireflies have constant velocity, and may pass freely through all  of space, including each other and you.  Let M(t) be the location of the  center of mass of the <strong>N</strong> fireflies at time t. Let d(t) be the distance between your position and M(t) at time t.  Find the minimum value of d(t), d<sub>min</sub>, and the earliest time when d(t) = d<sub>min</sub>, t<sub>min</sub>.</p>
<p><strong>Input</strong></p>
<p>The first line of input contains a single integer <strong>T</strong>, the number of test cases. Each test case starts with a line that contains an integer <strong>N</strong>, the number of fireflies, followed by <strong>N</strong> lines of the form</p>
<pre>x y z vx vy vz</pre>
<p>Each of these lines describes one firefly: (x, y, z) is its initial position at time t = 0, and (vx, vy, vz) is its velocity.</p>
<p><strong>Output</strong></p>
<p>For each test case, output</p>
<pre>Case #X: d<sub>min</sub> t<sub>min</sub></pre>
<p>where <strong>X</strong> is the test case number, starting from 1. Any answer with absolute or relative error of at most <strong>10<sup>-6</sup></strong> will be accepted.</p>
<p><strong>Limits</strong></p>
<p>All the numbers in the input will be integers.<br> 1 �� <strong>T</strong> �� 100<br> The values of x, y, z, vx, vy and vz will be between -5000 and 5000, inclusive.</p>
<p>Large dataset</p>
<p>3 �� <strong>N</strong> �� 500</p>
<p>&nbsp;</p>
<p><strong>Sample</strong></p>
<div>
<table border="0">
<tbody>
<tr>
<td><br> <span>Input</span> <br>&nbsp;</td>
<td><br> <span>Output</span> <br>&nbsp;</td>
</tr>
<tr>
<td><code> 3<br> 3<br> 3 0 -4 0 0 3<br> -3 -2 -1 3 0 0<br> -3 -1 2 0 3 0<br> 3<br> -5 0 0 1 0 0<br> -7 0 0 1 0 0<br> -6 3 0 1 0 0<br> 4<br> 1 2 3 1 2 3<br> 3 2 1 3 2 1<br> 1 0 0 0 0 -1<br> 0 10 0 0 -10 -1<br> <br> </code></td>
<td><code> Case #1: 0.00000000 1.00000000<br> Case #2: 1.00000000 6.00000000<br> Case #3: 3.36340601 1.00000000<br> <br> </code></td>
</tr>
</tbody>
</table>
</div>
<p>Notes</p>
<p>Given <strong>N</strong> points (x<sub>i</sub>, y<sub>i</sub>, z<sub>i</sub>), their center of the mass is the point (x<sub>c</sub>, y<sub>c</sub>, z<sub>c</sub>), where:</p>
<pre>x<sub>c</sub> = (x<sub>1</sub> + x<sub>2</sub> + ... + x<sub>N</sub>) / N
y<sub>c</sub> = (y<sub>1</sub> + y<sub>2</sub> + ... + y<sub>N</sub>) / N
z<sub>c</sub> = (z<sub>1</sub> + z<sub>2</sub> + ... + z<sub>N</sub>) / N
</pre>