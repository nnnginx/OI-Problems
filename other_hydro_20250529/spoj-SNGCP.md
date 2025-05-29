<p>Let <strong>num(num &gt;= 0) </strong>is a positive integer or zero. We can represent num in the following two forms if it is possible to do so -<br><strong>1.</strong> <strong>num = n<sup>2</sup> + 2 * n, for non-negative integer n</strong><br><strong>2.</strong> <strong>num = m<sup>2</sup> - 2 * m, </strong><strong>for non-negative integer m<br></strong></p>
<p>Suppose there is <strong>num</strong> that can be represented in both the forms. Consider this type of number as a magic number. Consider the following 5 cases -<br><strong>1. n is the only prime.<br>2. m is the only prime.<br>3. n and m both are primes.<br>4. n is prime.<br>5. m is prime.</strong></p>
<h3>Input</h3>
<p>First line of input is t, total number of test cases. For each test  case the first line is q, total number of queries. Then there will be (2  * q) lines. First line contains c (referring to case mentioned in the  problem description) and second line contains two integers a and b  defining the range <strong>[a, b] </strong>for magic number.<br><strong>t &lt; 1001<br>q &lt; 5001<br>0 &lt; c &lt; 6<br>minimum_value_of_a = 0<br>maximum_value_of_b = 10<sup>6</sup></strong></p>
<h3>Output</h3>
<p>For every test case, that has q queries, the output has (q + 1)  lines. First line will be simply printing the test case number and then q  lines will be printing total number of magic numbers in the given range  [a, b] under the specific case mentioned in input.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br><span style="color: #0000ff;">3<br>1<br>5 20<br>2<br>1 30<br>3<br>10 18<br></span><span style="color: #ff0000;">2<br>4<br>1 10<br>5<br>1 10
</span>
<strong>Output:</strong>
Test Case :#1:<span style="color: #0000ff;"><br>Query :#1: 1<br>Query :#2: 1<br>Query :#3: 1</span><br>Test Case :#2:<br><span style="color: #ff0000;">Query :#1: 1<br>Query :#2: 1<br><strong></strong></span></pre>