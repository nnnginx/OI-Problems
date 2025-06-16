<p>Let us consider the set of integer numbers between 1 and N inclusive. Order them lexicographically (i. e. like in the vocabulary), for example, for  N&nbsp;=&nbsp;11 the order would be: 1, 10, 11, 2, 3, 4, 5, 6, 7, 8, 9.</p>
<p>Denote the position of the number K in this ordering as Q<sub>N,K</sub>.  For example, Q<sub>11,2</sub>&nbsp;=&nbsp;4.</p>
<p>Given N and K, compute Q<sub>N,K</sub>.</p>
<h3>Input</h3>
<p>The first line contains a number T, which is the number of test cases. T lines follow, each contains 2 integers N and K separated by a single space.</p>
<h3>Output</h3>
<p>For each test case, print Q<sub>N,K</sub> on a single line.</p>
<h3>Constraint</h3>
<p>1 ¡Ü T ¡Ü 100</p>
<p>1 ¡Ü K ¡Ü N ¡Ü 10<sup>100</sup></p>
<h3>Example</h3>
<pre><strong>Input:</strong> <br>7<br>1 1<br>11 2<br>215 211<br>215 215<br>215 26<br>215 99<br>1000000000 999999999<br><br><strong>Output:</strong> <br>1<br>4<br>126<br>130<br>135<br>215<br>1000000000
</pre>