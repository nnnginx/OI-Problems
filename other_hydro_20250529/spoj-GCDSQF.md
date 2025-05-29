<p>
A number is <a title="Square-free" href="http://en.wikipedia.org/wiki/Square-free_integer">square-free</a> if its prime descomposition contains no repeated factors. For example: 1001 = 7 * 11 * 13 is square-free, but 20 = 2 * 2 * 5 is not square-free.
</p>
<p>
Square-free numbers can encoding as binary numbers. Here are examples to illustrate: <br>
<br>
Sequence of prime numbers 2 3 5 7 11 13 17 ... 
</p><ul>
  <li>42 = 2 * 3 * 7     &lt;=&gt; 1101</li>
  <li>1001 = 7 * 11 * 13 &lt;=&gt; 000111</li>
  <li>10 = 2 * 5         &lt;=&gt; 101</li>
</ul>
<p></p>

<p>
Your task is given two square-free integers A and B in binary representation compute gcd (A + B, lcm (A, B)). If the result is a square-free number your answer should have the binary format, if the answer&nbsp;is 1 print "relatively prime", and if is neither of these two cases print the result in base 10.
</p>

<h3>Input</h3>
<p>In the first line an integer T (1 &lt;= T &lt;= 100) the number of test cases.
The following 2 * T lines will appear integers A and B. The length of the integers A and B encoded in binary form must not exceed 1000 characters.
</p>

<h3>Output</h3>
<p>
For each of the T pairs A, B print in the specified format gcd (A + B, lcm (A, B)).
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
000111
101
11
011

<strong>Output:</strong>
relatively prime
01</pre>

<p><strong>Note:</strong>
In the input may have unnecessary zeros on the right of the numbers A and B, but Your answer only must be with necessary zeros.
</p>