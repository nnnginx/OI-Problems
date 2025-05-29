<p>Given a set of integers S = { a<sub>1</sub>, a<sub>2</sub>, a<sub>3</sub>, ... a<sub>|S|</sub> }, we define a function X on S as follows:<br>X( S ) = a<sub>1</sub> ^ a<sub>2</sub> ^ a<sub>3</sub> ^ ... ^ a<sub>|S|</sub>.<br>(^ stands for bitwise 'XOR' or 'exclusive or')</p>
<p>Given a set of N integers, compute the maximum of the X-function over all the subsets of the given starting set.</p>
<h3>Input</h3>
<p>The first line of input contains a single integer N, 1 &lt;= N &lt;= 10<sup>5</sup>.<br>Each of the next N lines contain an integer a<sub>i</sub>, 1 &lt;= a<sub>i </sub>&lt;= 10<sup>18</sup>.</p>
<h3>Output</h3>
<p>To the first line of output print the solution.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3<br>1<br>2<br>4<br><br><strong>Output:</strong><br>7</pre>