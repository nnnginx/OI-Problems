<p>Given <strong>N</strong>, find the largest number <strong>X</strong> not greater than <strong>N</strong> such that <strong>X</strong> is prime friendly. A number is called prime friendly when it satisfies both of the following conditions:
<br><br>
</p><ol>
  <li>The number itself is a prime.</li>
  <li>All its digits in base <strong>10</strong> are also primes. In other words, the number consists of only the digits <strong>2, 3, 5, 7.</strong></li>
</ol> 
<br><br>

<h3>Input</h3>
<p>The first line contains an integer <strong>T</strong>, denoting the number of test cases. Each test case contains a single positive integer <strong>N</strong>.

</p><h3>Constraints</h3>
<strong><li>1 &lt; T ¡Ü 1000</li></strong>
<strong><li>1 &lt; N ¡Ü 10<sup>18</sup></li></strong>

<h3>Output</h3>
<p>For each test case, output the case number followed by the largest number <strong>X</strong> not greater than <strong>N</strong>. Please refer to the sample input/output section for more clarity of the format.

</p><h3>Example</h3>

<pre><b>Input:</b>
5
10
100
1000
10000
100000


<b>Output:</b>
Case 1: 7
Case 2: 73
Case 3: 773
Case 4: 7757
Case 5: 77773
</pre>