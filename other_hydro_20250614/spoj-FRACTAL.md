<p>The Hilbert Mole is a small and very rare mole. The first and only specimen was found by David Hilbert
at his backyard. This mole lives in a huge burrow under the ground, and the border of this burrow forms
a Hilbert curve of n-th order (H<sub>n</sub>).</p>
<img src="./22475/file/0UU3KhQo.png">
<p>Figure 1.  Hilbert curves, order 1 to 4.</p>
<p>Hilbert curves can be defined as follows. H<sub>1</sub> is a unit square with open top side (figure 1(a)), H<sub>n</sub> consists
of four copies of H<sub>n-1</sub>: bottom left and bottom right are copied without changes, top left is rotated 90<sup>o</sup> counter-clockwise and top right is rotated 90<sup>o</sup> clockwise. These small copies are connected by three segments of unit length (figure 1(b),(c),(d)).</p>
<img src="./22475/file/5zoUa3i7.png">
<p>Figure 2.  Burrow, filled with water.</p>
<p>Trying to exterminate the mole, Mr. Hilbert fills the burrow with water (figure 2). But air inside the burrow
prevents water from filling it entirely. In this problem we suppose that air and water are incompressible
and cannot leak throw the borders of the burrow. Your task is to find the total area of the burrow, filled
with water.
</p><p>Note that water can flow over the obstacle only when its level is strictly higher. See examples on figure 3
for further clarification.</p>
<img src="./22475/file/EKhebPTW.png">
<p>Figure 3.  More examples of filled burrows.</p>
<h3>Input</h3>
<p>Multiple test cases. For each test case:
</p><p>The first line of the input file contains two integer numbers: n and alpha - order of Hilbert curve and slope angle of surface in degrees (1 &lt;= n &lt;= 12, 0 &lt;= alpha &lt; 90).
</p><p>Input terminates by EOF.</p>
<h3>Output</h3>
<p>For each test case:
</p><p>The first line of the output file must contain a single real number - the total area of the burrow, filled
with water. The relative error of the answer must not exceed 10<sup>-6</sup>.</p>
<h3>Example</h3>
<pre><b>Input:</b>
5 30
3 45
4 10
3 0

<b>Output:</b>
190.803847577293
15.5
91.573591766702
26.0
</pre>