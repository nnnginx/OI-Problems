<p>Johnny has created a table which encodes the results of some operation -- a function of two arguments. But instead of a boring multiplication table of the sort you learn by heart at prep-school, he has created a GCD (greatest common divisor) table! So he now has a table (of height <var>a</var> and width <var>b</var>), indexed from (1,1) to (<var>a</var>,<var>b</var>), and with the value of field (<var>i</var>,<var>j</var>) equal to gcd(<var>i</var>,<var>j</var>). He wants to know how many times he has used prime numbers when writing the table.</p>
<h3>Input</h3>
<p>First, <var>t</var> ¡Ü 10, the number of test cases. Each test case consists of two integers, 1 ¡Ü <var>a</var>,<var>b</var> &lt; 10<sup>7</sup>.</p>
<h3>Output</h3>
<p>For each test case write one number - the number of prime numbers Johnny wrote in that test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
10 10
100 100

<strong>Output:</strong>
30
2791</pre>