<p>The problem description is the same as the problem <a href="http://www.spoj.com/problems/DRAGON">DRAGON</a>.</p>
<h3>Input</h3>
<p>The first line contains 3 integers N(1&lt;=N&lt;=3000),M(2&lt;=M&lt;=N),K(1&lt;=K&lt;=N), separated by single spaces. The N fruits are numbered 1..N, and the biggest fruit is always numbered 1. N-1 lines follow, each contains 3 integers i,j,k separated by spaces denoted that there is a branch between fruit i(1&lt;=i&lt;=N) and fruit j(1&lt;=j&lt;=N) and the weight of illness of this branch is k(0&lt;=k&lt;=100000).</p>
<h3>Output</h3>
<p>Output one line contains a single integer denoted the minimum weight of illness of the hydra. If we can't divide the fruit into M groups, output "-1"(without quotes).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
8 2 4
1 2 20
1 3 4 
1 4 13
2 5 10
2 6 12
3 7 15
3 8 5

<strong>Output:</strong>
4
</pre>
<p><b>Some new test cases were added.</b></p>