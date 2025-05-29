<p><span style="font-size: small;"> The description of this problem is extremely simple. You are given <strong>2   non-intersecting circles</strong> in 3-dimensional world. Each of the circle is defined   by <strong>3 non - collinear points</strong> lying on the circle. All you have to return is   whether the circles are entangled or not (just like two links of a chain). Two   circles are entangled if they cannot be separated from each other without   breaking any of the circles. </span></p>
<h3><span style="font-size: small;">Input Format:</span></h3>
<p><span style="font-size: small;"> The first line contains a single integer, <strong>T</strong>, the number of test cases. Each of   the <strong>T</strong> test cases are defined by <strong>2</strong> lines. The first line of each test case   contains <strong>9</strong> integers representing the <strong>3</strong> points as <strong>(x1, y1, z1), (x2, y2, z2),   (x3, y3, z3)</strong> which define the first circle. Similarly, the second line for   each test case contains <strong>9</strong> integers representing the <strong>3</strong> points which define the   second circle. </span></p>
<h3><span style="font-size: small;">Output Format:</span></h3>
<p><span style="font-size: small;"> For every query output <strong>"YES"</strong> without quotes if the circles are entangled and   <strong>"NO"</strong> otherwise (quotes for clarity). </span></p>
<h3><span style="font-size: small;">Constraints:</span></h3>
<p><span style="font-size: small;"><strong> 1 ¡Ü T ¡Ü 100<br> -10000 ¡Ü Each Coordinate in the Input ¡Ü 10000</strong> </span></p>
<h3><span style="font-size: small;">Sample Input:</span></h3>
<pre><span style="font-size: small;">1
0 1 0 1 0 0 0 -1 0
0 0 0 1 0 -1 1 0 1</span></pre>
<h3><span style="font-size: small;">Sample Output:</span></h3>
<pre><span style="font-size: small;">YES</span></pre>
<p><span style="font-size: small;"><br> <strong>Problem Setter: Lalit Kundu</strong></span></p>