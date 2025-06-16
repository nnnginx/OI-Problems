<p>Blue Mary extremely like lemon trees. When the softness moon shines the ground, she lies under the lemon tree, thinking about the true meaning of life, the universe and everything quietly.</p>
<p>Before long, she is shadowed by the lemon tree. Blue Mary is such a cute girl, that she soon comes up with a question: what is the area of the shadow?</p>
<p>She knows it's hard for her to measure the shadow directly. So that, she tries to calculate it in geometrical way.</p>
<p>As Mary knows well about this beautiful lemon tree, she regards it as N frustums of cones,each frustums of cone is defined as a floor, numbered 1..N from the bottom to top. Of course, the Nth(Top) is a cone. Each frustum has two circle surfaces. Each two adjacent frustums shares a same circle surface. All the centres of the circle surfaces are on a plumb line. Mary knows that the height of every frustums is h1,h2,..,hn, and the undersurface of the 1st frustum has a height h0 from the ground.</p>
<p>Mary measures that the included angle of the moonshine and the ground is Alpha, which is an acute angle.</p>
<p><img src="../../../content/john_jones:lemon1.bmp" alt=""><img src="../../../content/john_jones:lemon2.bmp" alt=""></p>
<p>For briefness, we suppose the moonshine is parallel and the ground is aclinic.</p>
<p>And we ignore the bole of the tree. Mary comes up with the answer quickly, and she wants your ideas all the same.</p>
<h3>Input</h3>
<p>The very first line of the input data contains one integer T, the number of tests. T blocks follow.</p>
<p>For each test:</p>
<p>The first line of the input data contains one integer number N(N&lt;=500) and a real number Alpha (Alpha&gt;0.3).</p>
<p>N denote the number of floors, Alpha denote the included angle of the moonshine and the ground(radian).</p>
<p>The second line contains N + 1 real number h0 h1 h2... hn.(hi&lt;=100) h0 denotes the height of the undersurface of the 1st frustum. h1 .. hn denote the height of each floor.</p>
<p>The third line contains N real number r1 r2 .. rn(ri&lt;=100), the radii of the undersurface in  each floor.</p>
<p>All the data in each line is seperated by spaces.</p>
<h3>Output</h3>
<p>For each data set you should output one line containing a single real number - the area of the shadow. Numbers should be rounded to two decimal places.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
2 0.7853981633
10.0 10.00 10.00
4.00 5.00

<strong>Output:</strong>
171.97
</pre>