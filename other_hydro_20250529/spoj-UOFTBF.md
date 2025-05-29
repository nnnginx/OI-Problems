<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Having been sucked into your father's secret computer through a projector in the back of his arcade (or something), you find yourself in the wonderful world of Tron! Here, you play games all day, and if you ever lose, you die.</p>
<p>One such game involves you and an opponent driving around a flat grid on light cycles, which leave behind a permanent trail of...light...wherever they go. This grid can be modeled with the Cartesian plane, and is enclosed by a rectangle of impenetrable walls which ensure that the x-coordinate of each light cycle is always between $1$ and $10^{12}$, while its y-coordinate is between $1$ and $10^6$ (inclusive). Light cycles always stay on the grid lines, and move at a speed of 1 square per second.</p>
<p>A match lasts $S$ ($1 \leq S \leq 10^{100}$) seconds. You start at coordinates ($X_A$, $Y_A$) and follow a set of $N_A$ ($1 \leq N_A \leq 10^5$) instructions, with your $i$th instruction consisting of moving $L_{Ai}$ squares in the direction given by the character $D_{Ai}$ (with "U", "D", "L", and "R" representing up, down, left, and right, respectively). Similarly, your opponent starts at coordinates ($X_B$, $Y_B$) and follows a set of $N_B$ ($1 \leq N_B \leq 10^5$) instructions, with their $i$th instruction described by $L_{Bi}$ and $D_{Bi}$. Of course, neither player's instructions will ever take them beyond the boundaries of the walls, and it will take each player exactly $S$ seconds to execute their instructions. Additionally, for each player, no instruction will have an equal or opposite direction to that of their previous instruction. Finally, if a grid point is ever visited more than once throughout the course of the match, it is guaranteed that one of the path segments intersecting there is passing directly through vertically, while the other is passing directly through horizontally (as such, this cannot happen at either player's starting or ending points).</p>
<p>Whenever both light cycles reach the same grid point at the same time, or a light cycle hits an existing trail of light (in other words, a grid point which either light cycle had previously passed through), a collision occurs. Because you're just playing a practice match for now, neither player dies when this occurs, and, in fact, the collision is not counted in favour of either you or your opponent. Instead, for $T$ ($1 \leq T \leq 20$) scenarios as described above, you're simply interested in the number of collisions that will occur throughout each match.</p>
<h3>Input</h3>
<p>First line: 1 integer, $T$</p>
<p>For each scenario:</p>
<p>First line: 1 integer, $S$</p>
<p>Next line: 3 integers, $X_A$, $Y_A$, and $N_A$</p>
<p>Next $N_A$ lines: 1 character, $D_{Ai}$, and 1 integer, $L_{Ai}$, for $i = 1..N_A$</p>
<p>Next line: 3 integers, $X_B$, $Y_B$, and $N_B$</p>
<p>Next $N_B$ lines: 1 character, $D_{Bi}$, and 1 integer, $L_{Bi}$, for $i = 1..N_B$</p>
<h3>Output</h3>
<p>For each scenario:</p>
<p>1 integer: The total number of collisions that will occur.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">1<br>12<br>2 5 5<br>R 4<br>U 1<br>L 1<br>D 4<br>L 2<br>3 3 4<br>U 3<br>L 2<br>D 2<br>R 5</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">4</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The following diagram illustrates the paths of the light cycles (yours drawn in solid lines, and your opponent's drawn in dotted ones), as well as all of the collision points (indicated with large dots):</p>
<p><img src="../../../content/sourspinach:uoftbf.png" alt=""></p>