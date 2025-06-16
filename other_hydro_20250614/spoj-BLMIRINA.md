<p>Mirana is an archer with superpower. Every arrow she shoots will get stronger the further it travels. Mirana is currently on the way to warzone.</p>
<p>Since the road is still a long way, Mirana remembers about when she's still in training. In each of her training, Mirana stands on the (0,0) point in a cartesian scale. From that point, she must shoot a circle centered in (<strong>x</strong>,<strong>y</strong>) with radius <strong>r</strong>. Everything happens in z=0.</p>
<p>To maximize the arrow's power, Mirana must shoot the furthest point of the enemy possible. Her arrow travels at the speed of light and will instantly stops the moment it touches the target. On the target, determine the coordinate point that Mirana has to shoot to get maximum power. If multiple coordinate exists, choose the one with the lower x value.</p>
<h3>Input</h3>
<p>First line is T, number of training (T&nbsp;<span style="text-decoration: underline;">&lt;</span>&nbsp;100000). Next T lines each contains 3 space separeted integers x, y, and r for each training (1 <span style="text-decoration: underline;">&lt;</span>&nbsp;r <span style="text-decoration: underline;">&lt;</span>&nbsp;x,y <span style="text-decoration: underline;">&lt;</span>&nbsp;1000)</p>
<h3>Output</h3>
<p>For each training, output a line containing the coordinate of the arrow's destination separated by space. Output until 6 digit after decimal point.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>1 1 1<br>2 2 1<br>4 5 2&nbsp;</pre>
<pre><strong>Output:</strong>
0.000000 1.000000<br>1.088562 2.411438<br>2.126155 5.699076</pre>