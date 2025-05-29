<p>
You are given a matrix of size&nbsp;<b>r</b> x <b>c</b>. Each of the elements can be either 0 or 1.&nbsp; In each operation you can flip any element of this matrix, i.e. convert 0 to 1 or convert 1 to 0. Your goal is to convert the matrix such that -
</p>
<ol>
  <li>Each of the rows will have the same number of 1s and</li>
  <li>Each of the columns will have the same number of 1s.</li>
</ol>
<p>What is the minimum number of operations required to achieve this?</p>

<h3>Input</h3>
<p>Input starts with a positive integer&nbsp;<b>T</b>&nbsp;(~1000) which indicates the number of inputs.</p>

<p>Each case starts with two integers&nbsp;<b>m</b>&nbsp;and&nbsp;<b>n</b>&nbsp;(1 &lt;= <b>r</b>, <b>c</b> &lt;= 40), here&nbsp;<b>r</b>&nbsp;is the number of rows and&nbsp;<b>c</b>&nbsp;is the number of columns of the matrix. Each of the next <b>m</b> lines will have <b>n</b> integers each, either 0 or 1.</p>

<h3>Output</h3>
<p>For each test case, output <code>¡°Case #: R¡±</code> in a single line, where <code>#</code> will be replaced by case number and&nbsp;<b>R</b>&nbsp;will be replaced by the minimum number of steps required to achieve the target matrix. Replace&nbsp;<b>R</b>&nbsp;by <code>-1</code> if it is not possible to reach target matrix.</p>

<h3>Example</h3>
<strong>Sample Input:</strong><p></p>
<pre>3
2 3
111
111
3 3
011
011
011
2 3
001
000</pre>

<p><strong>Sample Output:</strong></p>
<pre>Case 1: 0
Case 2: 3
Case 3: 1</pre>