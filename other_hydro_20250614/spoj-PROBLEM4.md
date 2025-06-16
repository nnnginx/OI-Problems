<h3>Problem 4: PRIMITIVEROOTS</h3>
<h4>Introduction to Primitive Roots</h4>
<p>a <strong>primitive root modulo <em>n</em></strong> is any number <em>g</em> with the property that any number <a href="http://en.wikipedia.org/wiki/Coprime">coprime</a> to <em>n</em> is <a title="Modular arithmetic" href="http://en.wikipedia.org/wiki/Modular_arithmetic#Congruence_relation">congruent</a> to a power of <em>g</em> modulo <em>n</em>.</p>

<p>The number 3 is a primitive root modulo 7. because</p>
<p><img style="vertical-align: middle;" src="file://UuURw6ug.png" alt=""></p>

<h3>Problem Statement</h3>
<p>Given a number n as input you¡¯ve to find the (product all the primitive roots of n) % n if n is prime.</p>

<h3>Input</h3>
<p>The first line consists of T the number of test cases followed by T lines. Each line consists of a prime number n.</p>

<h3>Output</h3>
<p>For each test case print the test case number followed by ¡®<code>:</code>¡¯ followed by (product of all primitive roots of n) % n. If it is not a prime then print ¡°<code>NOTPRIME</code>¡±</p>

<h3>Input Specifications</h3>
<p>1 &lt;= T &lt;= 100</p>
<p>3 &lt;= n &lt;= 10000</p>

<h3>Example</h3>
<p><strong>Sample Input</strong></p>
<pre>3
6
7
9</pre>

<p><strong>Sample Output</strong></p>
<pre>1:NOTPRIME
2:1
3:NOTPRIME</pre>

<p><strong>Description for test case #2:</strong></p>
<p>The primitive roots of 7 are 3 and 5. The product % 7 = 15%7&nbsp; =1</p>