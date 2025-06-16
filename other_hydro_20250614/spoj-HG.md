<p><strong>RK</strong> has received a homework assignment to compute the <strong>greatest common divisor</strong> of the two positive integers <strong>A</strong> and <strong>B</strong>. Since the numbers are quite large, the professor provided him with <strong>N</strong> smaller integers whose product is <strong>A</strong>, and <strong>M</strong> integers with product <strong>B</strong>.</p>
<p>RK would like to verify his result, so he has asked you to write a program to solve his problem. If the result is more than 9 digits long, output only the <strong>last 9</strong> digits.</p>

<h3>Input</h3>
<p>The first line of input contains the positive integer <strong>N</strong> (1 &lt;= <strong>N</strong> &lt;= 1000).</p>
<p>The second line of input contains <strong>N</strong> space-separated positive integers less than 10^9, whose product is the number <strong>A</strong>.</p>
<p>The third line of input contains the positive integer <strong>M</strong> (1 &lt;= <strong>M</strong> &lt;= 1000).</p>
<p>The fourth line of input contains <strong>M</strong> space-separated positive integers less than 10^9, whose product is the number <strong>B</strong>.</p>

<h3>Output</h3>
<p>The first and only line of output must contain the greatest common divisor of numbers <strong>A</strong> and <strong>B</strong>. If the result is more than 9 digits long, output only the last (least significant) 9 digits.</p>

<h3>Example</h3>
<p><strong>Input</strong></p>
<pre>3
2 3 5
2
4 5</pre>

<p><strong>Output</strong></p>
<pre>10</pre>

<p><strong>Input</strong></p>
<pre>3
358572 83391967 82
3
50229961 1091444 8863</pre>

<p><strong>Output</strong></p>
<pre>000012028</pre>

<p>First sample description: The greatest common divisor of numbers A = 30 and B = 20 equals 10.</p>