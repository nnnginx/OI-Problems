<p>There is a robot on the 2D plane. Robot initially standing on the position (0, 0). Robot can make a 4 different moves:</p>
<ol>
<li>Up (from (x, y) to (x, y + 1)) with probability <strong>U</strong>.</li>
<li>Right (from (x, y) to (x + 1, y)) with probability <strong>R</strong>.</li>
<li>Down (from (x, y) to (x, y - 1)) with probability <strong>D</strong>.</li>
<li>Left (from (x, y) to (x - 1, y)) with probability <strong>L</strong>.</li>
</ol>
<p>After moving <strong>N</strong> times Robot gets points.</p>
<ul>
<li>Let x<sub>1</sub>&nbsp;be the smallest coordinate in X-axis, that Robot reached in some moment.</li>
<li>Let x<sub>2</sub>&nbsp;be the largest coordinate in X-axis, that Robot reached in some moment.</li>
<li>Let y<sub>1</sub>&nbsp;be the smallest coordinate in Y-axis, that Robot reached in some moment.</li>
<li>Let y<sub>2</sub>&nbsp;be the largest coordinate in Y-axis, that Robot reached in some moment.</li>
</ul>
<p>Points achieved by Robot equals to x<sub>2</sub>&nbsp;- x<sub>1</sub>&nbsp;+ y<sub>2</sub>&nbsp;- y<sub>1</sub>.</p>
<p>Given <strong>N, U, R, D, L</strong>. Calculate <a href="https://en.wikipedia.org/wiki/Expected_value">expected value</a> of points that Robot achieved after <strong>N</strong> moves.</p>
<h3>Input</h3>
<p>First line: One interger <strong>N (1 ¡Ü N ¡Ü 200)</strong>.</p>
<p>Second line: Four real numbers <strong>U, R, D, L (U + R + D + L = 1, 0 ¡Ü U, R, D, L <strong>¡Ü 1</strong></strong>) with maximum of 6 numbers after dot.</p>
<h3>Output</h3>
<p>One number: expected value of points achieved by Robot. The answer will be considered correct if its relative or absolute error does not exceed 10<sup>-6</sup>.</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
2
0.100000 0.200000 0.300000 0.400000
<strong>Output:</strong>
1.780000</pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
3
0.25 0.25 0.25 0.25
<strong>Output:</strong>
2.375000</pre>