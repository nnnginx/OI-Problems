<p>G(n) is defined as</p>
<p>G(n) = G(n-1) + f(4n-1)   , for n &gt; 0</p>
<p>and    G(0) = 0</p>
<p>f(i) is ith Fibonacci number. Given n you need to evaluate G(n) modulo 1000000007.</p>

<h3>Input</h3>
<p>First line contains number of test cases t (t&lt;40000). Each of the next t lines contain an integer n ( 0 &lt;= n &lt; 2^51).</p>

<h3>Output</h3>
<p>For each test case print G(n) modulo 1000000007.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
2
4</pre>

<pre><strong>Output:</strong>
15
714</pre>