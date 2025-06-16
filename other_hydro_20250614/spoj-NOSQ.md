<p>A square free number is defined as a number which is not divisible by any square number.</p>
<p>For example, 13, 15, 210 are square free numbers, where as 25 (divisible by 5*5), 108 (divisible by 6*6), 18 (divisible by 3*3) are not square free numbers. However number 1 is not considered to be a square and is a squarefree number.</p>
<p>Now you must find how many numbers from number a to b, are square free and also have a digit d inside it.</p>
<p>For example for in the range 10 to 40 te squarefree numbers having digit 3 are 13, 23, 30, 31, 33, 34, 35, 37, 38, 39</p>

<h3>Input</h3>
<p>The first line contains an integer T, which is the number of test-cases</p>
<p>Then follow T lines, each containing 3 integers a, b and d.</p>
<p>1 &lt;= T &lt;= 20,000</p>
<p>1 &lt;= a &lt;= b &lt;= 100,000</p>
<p>0 &lt;= d &lt;= 9</p>

<h3>Output</h3>
<p>Print one integer which is the required number as described in the problem statement.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
10 40 3
1 100 4
1 100000 7

<strong>Output:</strong>
10
9
26318</pre>