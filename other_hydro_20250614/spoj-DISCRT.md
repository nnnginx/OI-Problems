<p>In this problem, we try to compute discrete k<sup>th</sup>&nbsp;root modulo n; given n, k, a; find all the solutions for x such that x<sup>k</sup>&nbsp;= a (mod n) and x is coprime with n.</p>
<h3>Input</h3>
<p>For each input file, there are 3 space seperated integers n, k, a.</p>
<p>n = p<sup>e</sup>&nbsp;for some odd prime p, integer e &gt; 0; 0 &lt;= a &lt; n &lt;= 10<sup>9</sup>, 0 &lt;= k &lt; phi(n), where phi is Euler's totient function; the numbers n, a are coprimes.</p>
<h3>Output</h3>
<p>The first line of the output contains a single integer m, the number of solutions in the range [0, n - 1] that are coprimes with n, followed by m lines that contain the m solutions in ascending order. It is guranteed that m &lt;= 10<sup>4</sup>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 1 3

<strong>Output:</strong></pre>
<pre>1
3</pre>