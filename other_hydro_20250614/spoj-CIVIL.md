<!-- p { margin-bottom: 2.12mm; } -->
<p>Civil engineers are people who build impressive structures from concrete and steel. Throughout the world, sky scrapers get ever higher, bridges get ever wider, and tunnels get ever longer. Most recently, the Gotthard Base Tunnel just pushed the limits a bit further...</p>
<p style="text-align: center;"><img src="../../../content/jbw:gotthard_small.jpg" alt="Gotthard base tunnel" width="400" height="225"></p>
<!-- p { margin-bottom: 2.12mm; } -->
<p>In this task, you take the role of a civil engineer who is to build a tunnel through a mountain. Unfortunately, you have a very limited budget, and must construct the cheapest possible tunnel.</p>
<p>Because engineers have a habit of simplifying things, we will model the mountain and the tunnel using basic geometric shapes. First of all, consider that the earth is flat, and two-dimensional. On this flat surface stands a mountain of height h and width w. Each side of the mountain is parabolic (i.e. satisfies y = ax² + bx + c for some a, b, c). You also know that the base of the mountain is smooth, which means that its steepness at the base is zero.</p>
<p style="text-align: center;"><img src="../../../content/jbw:tunnel_small.png" alt="Graphical view of a tunnel" width="400" height="279"></p>
<p>The tunnel is modeled as a horizontal line through the mountain. The best possible tunnel is the one which minimizes construction cost. This cost is proportional to the length of the road which leads to the tunnel, plus the length of the tunnel itself. Consider that each meter of the tunnel is a factor f times as expensive as a meter of road.</p>
<h3>Input</h3>
<!-- p { margin-bottom: 2.12mm; } -->
<p>The input file consists of several test cases. Each case is given on a line by itself and consists of the three numbers h, w and f, separated by a space. All these are strictly positive floating point numbers. The input file ends with a test case where all numbers are zero (which must not be processed).</p>
<h3>Output</h3>
<!-- p { margin-bottom: 2.12mm; } -->
<p>Print for each test case a single number, the optimal height t of the tunnel. Always print three digits after the decimal point. You may assume that it is always cheaper to build some tunnel than to drive over the top of the mountain.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 2 1.5
9033.66 29752.4 1.56382
0 0 0<strong><br><br>Output:</strong><br><!-- p { margin-bottom: 2.12mm; } -->0.313<br>8852.956<br></pre>