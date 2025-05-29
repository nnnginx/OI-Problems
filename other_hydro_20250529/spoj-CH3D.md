<p>Bytelandian scientists have developed a brand new method for determining the volume of a person's lungs. The idea is simple: the patient is asked to inhale a sufficiently large number of nanobots, which then transmit their exact 3D-coordinates to an external sensor. Early clinical tests proved rather fun (especially for the scientists who were watching the process of nanobot inhalation), but gave rise to several problems of an algorithmic nature. In other words, nobody had any idea of how the volume of the lungs should be determined afterwards. A lung consists of a large number of disjoint alveoli (which can for our purposes be regarded as little hollows), and inhaled nanobots tend to float around aimlessly within the alveolus they happened to fall into. Whereas it is relatively simple to distinguish between different alveoli, establishing the volume of a single alveolus is a tough task.

</p><p>One way to estimate the shape and volume of an alveolus is to smear all nanobots with a little liquid glue and see what they end up stuck to. Another (arguably more humane) method is to calculate the <i>convex hull</i> of the set of points representing nanobot coordinates, its volume and surface area. A convex hull of given set of points in 3D is the convex set of minimum volume which contains all these points.
<br>

</p><center><img src="/content/turbo:ch3d_lung1.jpg" alt="Lung 1"><br>
<img src="/content/turbo:ch3d_arrow.jpg" alt="arrow"><br> <img src="/content/turbo:ch3d_lung2.jpg" alt="Lung 2"><br> 
<img src="/content/turbo:ch3d_arrow.jpg" alt="arrow"><br> <img src="/content/turbo:ch3d_lung3.jpg" alt="Lung 3"></center>
<p></p>

<h3>Input</h3>
<p><i>t</i> ¨C number of test cases [<i>t</i> &lt;= 100], then <i>t</i> tests follow.<br> Each test starts with integer <i>N</i> - the number of given points [10 &lt;= N &lt;= 1000]. Then exactly N lines follow with 3 real numbers Xi, Yi, Zi in each of them, where [-10.0 &lt;= Xi, Yi, Zi &lt;= 10.0].
</p>

<h3>Output</h3>
<p>For each test case you should output 2 real numbers: the surface area and volume of the hull with precision 0.01.

</p><h3>Example</h3>
<pre><b>Input:</b>
1
10
0.00000 0.00000 0.00000
1.00000 0.00000 0.00000
0.00000 1.00000 0.00000
0.00000 0.00000 1.00000
1.00000 1.00000 0.00000
1.00000 0.00000 1.00000
0.00000 1.00000 1.00000
1.00000 1.00000 1.00000
0.50000 0.50000 0.50000
0.66666 0.77777 0.88888

<b>Output:</b>
6.0000 1.0000

</pre>