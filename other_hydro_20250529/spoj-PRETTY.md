<p>Let S = {1, 2, 3, ..., N}.<br>For a given positive integer K, the function f : S --&gt; S is called "pretty" if, for every X in S, it holds that<br>f ( f ( f ( ... f ( X ) ... ) ) ) = X, where f is repeated exactly K times.<br> <br>How many pretty functions are there, modulo M?</p>
<h3>Input</h3>
<p>Three natural numbers N, K and M. It holds that 1 &lt;= K &lt;= N &lt;= 30 000 and M &lt;= 10^9.</p>
<h3>Output</h3>
<p>Number of pretty functions modulo M.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2 1<br>1000<br><br><strong>Output:</strong><br>1</pre>
<pre><strong>Input:</strong><br>3 2<br>1000<br><br><strong>Output:</strong><br>4</pre>
<p>Explanation of the example input 2: there are four pretty functions, namely:<br>a) f(1) = 1, f(2) = 2, f(3) = 3; <br>b) f(1) = 2, f(2) = 1, f(3) = 3;<br>c) f(1) = 3, f(2) = 2, f(3) = 1;<br>d) f(1) = 1, f(2) = 3, f(3) = 2.</p>
<p>&nbsp;</p>