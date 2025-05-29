<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Doctor Y, a leading expert in the field of boxology, is investigating the properties of boxen with his expensive super-precision laser. In particular, he plans to position the laser inside the union of a bunch of boxen, and see where the beam collides with itself.</p>
<p>Since Doctor Y blew all his cash on the laser, he can＊t actually afford to purchase boxen to conduct his experiment 每 instead, he will simulate it on his old computer, which uses an integer grid system. He will give his computer an integer $N$, the number of boxen ($1 \leq N \leq 10,000$), as well as their descriptions. Each box is described by 4 integers, $x_1$, $y_1$, $x_2$, and $y_2$, and is an axis-aligned rectangle with coordinates ($x_1$, $y_1$) and ($x_2$, $y_2$) describing a pair of its opposite corners. Boxen may overlap with one another. He will also input the location of the laser ($A$, $B$), such that it will be positioned strictly within at least one of the boxen. The laser points down and right at a 45～ angle. All coordinates have absolute values of at most $3000$.</p>
<p>As it turns out, boxen are made of a perfectly reflective material (a fact which Doctor Y will discover upon completion of his experiment) 每 as such, whenever the laser beam hits the edge of the union of the boxen, it bounces off. For example, if it hits a vertical edge from the left, it bounces to the right, with the up-down direction preserved. If it hits a corner head-on, it will reverse direction, hence colliding with itself right at the corner. Normally, light travels quite fast, but due to the mysterious properties of boxen, the speed of light when inside a box union is only ﹟2 units/second.</p>
<p>Doctor Y plans to use his computer to simulate the path of the laser and see when and where it first collides with itself, but there＊s one problem 每 he doesn't know how to program! Offering non-cafeteria food, he lures a desperate Waterloo student into his lab, where he forces him (or her?) to write the laser simulation program. That＊s you.</p>
<h3>Input</h3>
<p>Line $1$: 1 integer, $N$</p>
<p>Line $2$: 2 integers, $A$ and $B$</p>
<p>Next $N$ lines: 4 integers, $x_1$, $y_1$, $x_2$, and $y_2$, describing the coordinates of each box</p>
<h3>Output</h3>
<p>If the laser beam never collides with itself or the laser, simply output ※Time limit exceeded§.</p>
<p>If the laser beam collides with the actual laser (at coordinates ($A$, $B$)) before it collides with another location through which the beam has already passed, the first line of output should consist of a single number 每 the amount of time that passes before laser beam collides with the laser, in seconds. The second line should read ※Broken equipment§.</p>
<p>Otherwise, the first line of output should consist of a single number 每 the amount of time that passes before laser beam first collides with itself, in seconds. The second line should contain a pair of numbers 每 the x and y coordinates of where this takes place.</p>
<p>Each number should be rounded off to 1 decimal place.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">7</span>
<span style="font-family: 'courier new', courier;">0 4</span>
<span style="font-family: 'courier new', courier;">-1 5 1 -1</span>
<span style="font-family: 'courier new', courier;">0 -2 4 2</span>
<span style="font-family: 'courier new', courier;">0 -4 1 2</span>
<span style="font-family: 'courier new', courier;">2 -4 5 -1</span>
<span style="font-family: 'courier new', courier;">5 2 7 4</span>
<span style="font-family: 'courier new', courier;">3 -5 4 -4</span>
<span style="font-family: 'courier new', courier;">0 -6 3 -4</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">12.0</span>
<span style="font-family: 'courier new', courier;">0.0 0.0</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The grid looks like this:</p>
<p><img src="../../content/sourspinach:ulaser.bmp" alt="" width="275" height="325"></p>
<p>The filled-in squares represent squares that are part of at least one box 每 together, they make up the box union. Note that the union can have holes in it, and that it can be disjoint.</p>
<p>The blue lines denote the boundaries of the union 每 these are the lines that the laser can bounce off of.</p>
<p>The yellow lines are edges of boxen that do not contribute to the union 每 the laser can go through these freely.</p>
<p>The red diamond is the position of the laser, and the red line is the path that the laser beam follows. Note that when it bounces off the corner at (2,-2), since it didn＊t hit it head-on, it is the same as bouncing off of a horizontal edge.</p>
<p>Following the path of the laser beam, it can be seen that it collides with itself at (0,0). Before this, it has travelled 12﹟2 units, which takes exactly 12 seconds.</p>
<pre><strong>More Examples:</strong></pre>
<p>If the laser were positioned at (0,3), the output should be:</p>
<pre><span style="font-family: 'courier new', courier;">12.0<br></span><span style="font-family: 'courier new', courier;">0.0 -1.0</span></pre>
<p>&nbsp;If the laser were positioned at (0,1), the output should be:</p>
<pre><span style="font-family: 'courier new', courier;">5.0<br></span><span style="font-family: 'courier new', courier;">5.0 -4.0</span></pre>
<p>&nbsp;If the laser were positioned at (0,0), the output should be:</p>
<pre><span style="font-family: 'courier new', courier;">8.0<br></span><span style="font-family: 'courier new', courier;">Broken equipment</span></pre>