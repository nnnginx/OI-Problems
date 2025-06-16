<p>Count the number of distinct expressions involving <em>n</em> different operands <strong>a</strong>, <strong>b</strong>, <strong>c</strong>, etc. Only operators +, -, *, / and parentheses are permitted. Single minus operator (for ex. -a*b) is not allowed.</p>
<p>Two expression are distinct if for some valid input values (i.e. You won't divide some number by zero) <strong>a</strong>, <strong>b</strong>, <strong>c</strong>, ... , the two expressions leads to different results. For example, a/b/c and a/(b*c) are the same expressions, but a/b+c and a/(b+c) are not.</p>
<h3>Input</h3>
<p>Multiply test cases. For each test case:</p>
<p>A single line - <em>n</em>.(1&lt;= <em>n</em> &lt;=50).</p>
<p>Input terminates by a single zero.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>The number of different expressions, modulo 499999999999993.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
0

<strong>Output:</strong>
68
</pre>

<p>If you find the constraints is too small in this problem, try problem <a href="http://spoj.com/problems/EXPR4">EXPR4</a>.</p>