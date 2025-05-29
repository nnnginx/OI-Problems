<p>For a sequence of N integers, A1, A2, ..... AN</p>
<p>We can calculate the stability factor P,&nbsp;as</p>
<p>P = sum of all (abs(A<sub>i</sub>-A<sub>i-1</sub>)*C[i]) where 2 &lt;= i &lt;= N</p>
<p>C[i] is the cost of putting a number at position i</p>
<p>Your task is find the minimum P for the given N numbers considering all the different permutations of them.</p>
<p><strong>Input</strong></p>
<p>First line contains an integer T(1&lt;=T&lt;=10) which denotes the total number of test cases. Each test case consists of three lines.</p>
<p>The first line contains the integer N(1&lt;=N&lt;=15). The second line contains a space separated list of N integers(&lt;150)&nbsp;which denote the given set of numbers.</p>
<p>The third line contains a space separated list of N integers. The ith integer on this line denotes the value for C[i](1 &lt;= C[i] &lt; 150)</p>
<h3>Output</h3>
<p>For each test case, print the minimum possible value of P considering all permutations of the given numbers.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
5
1 8 3 6 5
1 2 3 4 5

<strong>Output</strong>
24
</pre>
<p>One of the possible permutation of given numbers which has p = 24 is 1, 3, 5, 6, 8</p>