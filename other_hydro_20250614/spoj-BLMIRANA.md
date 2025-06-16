<p>Mirana is an archer with superpower. Every arrow she shoots will get stronger the further it travels. Mirana is currently on a warzone.</p>
<p>Coincidentally, there's a guy selling mayonnaise. With the power of mayonnaise, Mirana's arrow can pierce every obstacle in its way. Unfortunately, there's only enough mayonnaise to power an arrow.</p>
<p>Mirana stands on the (0,0) point in cartesian scale. From that point she must shoot as many enemies as possible with an arrow. Each enemy has a circle shaped hitbox. An enemy dies if the arrow travels through its hitbox. Determine the maximum number of enemies that can be shot with an arrow!</p>
<h3>Input</h3>
<p>First line contains T, number of wars. On the i-th war, first line contains N<sub>i</sub>, number of enemies. Next N<sub>i</sub> lines each contains 3 space separated integers x, y, and r, the position and radius of the hitbox of each enemy.</p>
<ul>
<li>N<sub>i</sub>&nbsp;<span style="text-decoration: underline;">&lt;</span>&nbsp;125000</li>
<li>N<sub>1</sub> + N<sub>2</sub> + ... + N<sub>T</sub> <span style="text-decoration: underline;">&lt;</span>&nbsp;500000</li>
<li>1 <span style="text-decoration: underline;">&lt;</span>&nbsp;r <span style="text-decoration: underline;">&lt;</span>&nbsp;x <span style="text-decoration: underline;">&lt;</span>&nbsp;1000</li>
<li>-1000 <span style="text-decoration: underline;">&lt;</span>&nbsp;y <span style="text-decoration: underline;">&lt;</span>&nbsp;1000&nbsp;</li>
</ul>
<h3>Output</h3>
<p>For each war, output a line containing the maximum number of enemies that can be shot with an arrow.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>3<br>1 1 1<br>2 2 1<br>4 5 2<br>3<br>5 -4 1<br>10 -5 1<br>20 -10 1

<strong>Output:</strong>
3<br>2&nbsp;</pre>