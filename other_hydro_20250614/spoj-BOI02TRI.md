<p>There are given n isosceles right triangles on a plane. Each triangle can be described by three integers x,y,m (m&gt;0). Vertices of such a triangle are points which have coordinates (x;y), (x+m;y) and (x; y+m).</p>
<p>Write a program which calculates the total area covered by triangles.</p>
<h3>Input</h3>
<p>The first line of the input contains one positive integer n (n &lt;= 2000), the number of triangles on a plane.</p>
<p>The next n lines of the file describe the triangles, one triangle per line. Each line contains three integers x<sub>i</sub>, y<sub>i</sub> and m<sub>i</sub>, separated by single spaces (1 &lt;= i&nbsp;&lt;= n, ‑10<sup>7</sup>&nbsp;&lt;= x<sub>i</sub>&nbsp;&lt;= 10<sup>7</sup>, ‑10<sup>7</sup>&nbsp;&lt;= y<sub>i</sub>&nbsp;&lt;= 10<sup>7</sup>, 0&nbsp;&lt;&nbsp;m<sub>i</sub>&nbsp;&lt;= 1000).</p>
<h3>Output</h3>
<p>On the first line of the output one number with exactly one digit after decimal point must be written – the total area covered by triangles.</p>
<h3>Example</h3>
<div style="text-align: center;"><img style="vertical-align: middle;" src="../../../content/rlewon:BOI02TRI-fig1" alt="Triangles"></div>
<pre><strong>Input</strong>
5
-5 -3 6
-1 -2 3
 0 0 2
-2 2 1
-4 -1 2

<strong>Output</strong>
24.5
</pre>