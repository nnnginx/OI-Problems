The fibonacci series is defined as below:
<br><br>
<i>fib(0) = 0, fib(1) = 1</i>
<br><br>
<i>fib(n) = fib(n-1) + fib(n-2) for n &gt; 1</i>

<br><br>

Given three integers <strong>N</strong>, <strong>C</strong> and <strong>K</strong>, find the summation of the following series:
<br><br>
<strong><i>fib(0*C)^K + fib(1*C)^K + fib(2*C)^K + fib(3*C)^K + ¡­ + fib(N*C)^K</i></strong>
<br><br>
Since the answer can be huge, output it modulo <strong>1000000007</strong>
<br><br>

<h3>Input</h3>
The first line contains an integer <strong>T</strong>, denoting the number of test cases. Each test case contains three space separated integers in the order: <strong>N</strong>, <strong>C</strong> and <strong>K</strong>.


<h3>Constraints</h3>
<strong><li>1 ¡Ü T ¡Ü 100</li></strong>
<strong><li>0 ¡Ü <strong>N</strong> ¡Ü 10<sup>15</sup></li></strong>
<strong><li>1 ¡Ü C, K ¡Ü 10</li></strong>

<h3>Output</h3>
For each test case, output a single line in the format <i>¡°Case X: Y¡±</i> without the quotes. Here, <strong>X</strong> is the case number and <strong>Y</strong> is the desired answer denoting the sum of the series.

<h3>Example</h3>
<pre><b>Input:</b>
5
10 1 1
5 2 2
3 3 4
1000000007 7 9
996969696969696 9 6


<b>Output:</b>
Case 1: 143
Case 2: 3540
Case 3: 1340448
Case 4: 880410497
Case 5: 689328397

</pre>

<h3>Challenge</h3>
Try the harder version here:
<br><br>
<a href="https://www.spoj.com/problems/FIBPSUM2/">liouzhou_101 - FIBPSUM2</a>