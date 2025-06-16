<p>We all know about the classical fibonaaci series, Fibonacci series is F(n)=F(n-1)+F(n-2). For this question we call it a 2-Nacci series as a new element is calculated as the sum of the last 2 terms of the series. For fibonaaci we assume F(0)=0 and F(1)=1. We define as new series N-Nacci where F(n) is the sum of the last n terms and here we assume that F(0)=0, F(1)=1,F(2)=2... F(n-1)=(n-1). Your task is to calculate the last K digits of the Lth term of the N-Nacci series(no leading zeros needed).</p>
<p>&nbsp;</p>
<p>Constraints</p>
<p>&nbsp;</p>
<p>2&lt;=N&lt;=30</p>
<p>K&lt;=8</p>
<p>L&lt;=1000000000</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line of the input denotes the number of test cases t(atmost 10). Each line denotes a test case consisting of N,K,L.</p>
<h3>Output</h3>
<p>For each test case print the last K digits of the Lth term of the N-Nacci series.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4
2 1 5
3 6 12
4 1 10
4 2 10

<strong>Output:</strong></pre>
<pre>5
778
6
16
</pre>