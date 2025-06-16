<p><span style="font-size: medium;"><strong>Task</strong></span></p>
<p>You are given <strong>K</strong> points with positive integer coordinates. You are also given <strong>M</strong> triangles, each of them having one vertex in the origin and the other 2 vertices with non-negative integer coordinates.</p>
<p>You are asked to determine for each triangle whether it has at least one of the <strong>K</strong> given points inside. (None of the K points are on any edge of any triangle.)</p>
<p><span style="font-size: medium;"><strong>Input</strong></span></p>
<p>The first line of the input file will contain <strong>K</strong> and <strong>M</strong>. The following <strong>K</strong> lines will contain 2 positive integers <strong>x</strong> <strong>y</strong> separated by one space that represent the coordinates of each point. The next <strong>M</strong> lines have 4 non-negative integers separated by one space, (<strong>x1</strong>, <strong>y1</strong>) and (<strong>x2</strong>, <strong>y2</strong>), that represent the other 2 vertices of each triangle, except the origin.</p>
<p><span style="font-size: medium;"><strong>Output</strong></span></p>
<p>The output file should contain exactly <strong>M</strong> lines. The <em>k</em>-th line should contain the character <strong>Y</strong> if the <em>k</em>-th triangle (in the order of the input file) contains at least one point inside it, or <strong>N</strong> otherwise.</p>
<p><strong>Constraints</strong></p>
<ul>
<li>1 ≤ <strong>K</strong>,<strong>M</strong> ≤ 100 000</li>
<li>1 ≤ each coordinate of the <strong>K</strong> points ≤ 10<sup>9</sup></li>
<li>0 ≤ each coordinate of the triangle vertices ≤ 10<sup>9</sup></li>
<li>Triangles are not degenerate (they all have nonzero area).</li>
<li>In 50% of the test cases, all triangles have vertices with coordinates <strong>x1=0</strong> and<br><strong>y2=0</strong>. That is, one edge of the triangle is on the <em>x</em>-axis, and another is on the <em>y</em>-axis.</li>
</ul>
<p><span style="font-size: medium;"><strong>Sample input 1</strong></span></p>
<p><span style="font-size: small;"><span style="font-family: courier new,courier;">4 3<br>1 2<br>1 3<br>5 1<br>5 3<br>1 4 3 3<br>2 2 4 1<br>4 4 6 3</span></span></p>
<p><span style="font-size: medium;"><strong>Sample output 1</strong></span></p>
<p><span style="font-family: courier new,courier;"><span style="font-size: small;">Y<br>N<br>Y</span></span></p>
<p><span style="font-size: medium;"><strong>Explanation for sample 1</strong></span></p>
<p><img src="../../../content/andmej:tri1.png" alt="Explanation for sample 1" width="269" height="233"></p>
<p><span style="font-size: medium;"><strong>Sample input 2</strong></span></p>
<p><span style="font-size: small;"><span style="font-family: courier new,courier;">4 2<br>1 2<br>1 3<br>5 1<br>4 3<br>0 2 1 0<br>0 3 5 0</span></span></p>
<p><span style="font-size: medium;"><strong>Sample output 2</strong></span></p>
<p><span style="font-size: small;"><span style="font-family: courier new,courier;">N<br>Y</span></span></p>
<p><strong>Explanation for sample 2</strong></p>
<p><strong><img src="../../../content/andmej:tri2.png" alt="Explanation for sample 2" width="272" height="234"></strong></p>
<p><a href="http://www.ceoi2009.ro"><strong> 
</strong></a></p><hr><a href="http://www.ceoi2009.ro"><strong>
</strong></a><p></p>
<pre id="line1"><a href="http://www.ceoi2009.ro">CEOI 2009 - Tîrgu Mureş, Romania</a></pre>