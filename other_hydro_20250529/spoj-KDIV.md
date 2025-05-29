The <i>positive divisor function</i> is defined as a function that counts the number of positive divisors of an integer <strong>N</strong>, including <strong>1</strong> and <strong>N</strong>.
<br><br>

If we define the positive divisor function as <strong>D(N)</strong>, then, for example:

<br><br>
<strong>D(1) = 1</strong>
<br><br>
<strong>D(2) = 2</strong>
<br><br>
<strong>D(10) = 4</strong>
<br><br>
<strong>D(24) = 8</strong>
<br><br>

Calculating <strong>D(N)</strong> is a classical problem and there are many efficient algorithms for that. But what if you are asked to find something different? Given a range and an integer <strong>K</strong>, can you find out for how many <strong>N</strong> in the given range, <strong>D(N)</strong> equals <strong>K</strong>?

<br><br>

<h3>Input</h3>
In the very first line, you¡¯ll have an integer called <strong>T</strong>. This is the number of test cases that shall follow. Every test case contains three integers, <strong>L</strong>, <strong>R</strong>, and <strong>K</strong>. <strong>L</strong> and <strong>R</strong> represent the range and are inclusive.
<br><br>

<h3>Constraints</h3>
<strong></strong><li><strong>1 ¡Ü T &lt; 31</strong>
<strong></strong></li><li><strong>1 ¡Ü L ¡Ü R &lt; 2<sup>31</sup></strong></li>
<strong><li>1 ¡Ü K &lt; 2<sup>31</sup></li></strong>

<h3>Output</h3>
For every test case, you must print the case number, followed by the count of numbers with exactly <strong>K</strong> divisors in the range.

<h3>Sample Input</h3>
<pre>3
10 10 4
2 13 2
100 10000 100
</pre>

<h3>Sample Output</h3>
<pre>Case 1: 1
Case 2: 6
Case 3: 0
</pre>