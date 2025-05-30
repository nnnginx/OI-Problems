<p>The fibonacci sequence is defined by the following relation:</p>
<ul>
  <li>F(0) = 0</li>
  <li>F(1) = 1</li>
  <li>F(N) = F(N - 1) + F(N - 2), N &gt;= 2</li>
</ul>
<p>Your task is very simple. Given two non-negative integers N and M, you have to calculate the sum (F(N) + F(N + 1) + ... + F(M)) mod 1000000007.</p>

<h3>Input</h3>
<p>The first line contains an integer T (the number of test cases). Then, T lines follow. Each test&nbsp;case consists of a single line with two non-negative integers N and M.</p>

<h3>Output</h3>
<p>For each test case you have to output a single line containing the answer for the task.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
0 3
3 5
10 19

<strong>Output:</strong>
4
10
10857</pre>

<h3 style="font-size: 1.17em;">Constraints</h3>
<ul>
<li>T &lt;= 1000</li>
<li>0 &lt;= N &lt;= M &lt;= 10<sup>9</sup></li>
</ul>