<p>For <strong><em>n</em></strong> positive integer, let <strong><em>F(n) = 1! ¡Á 2! ¡Á 3! ¡Á 4! ¡Á ... ¡Á n!</em></strong>, product of factorial(i) for i in [1..n],<br>


<br>

For <strong><em>p</em></strong> a prime number, and <strong><em>n</em></strong> an integer,
and let <strong><em>V(p, n) = max({i&gt;=0 integer, such that p^i divides F(n)})</em></strong>. <br>




</p><h3>Input</h3>
<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.<br>
On each of the next <strong><em>T</em></strong> lines, your are given
two integers <strong><em>p</em></strong> a prime number, and <strong><em>e</em></strong>.
</p>

<h3>Output</h3>
<p>For each test case, you have to print <strong><em>V(p, p^e)</em></strong>.<br>
As the answer may not fit in a 64-bit container, just output your answer modulo 10^9+7.

</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1
2 2
</pre>
<pre><strong>Output:</strong>
5
</pre>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 10^5
1 &lt; p &lt; 10^18, a prime number
0 &lt; e &lt; 10^18
</pre>
<p><strong><em>p</em></strong> and <strong><em>e</em></strong> are log-uniform independent randomly distributed. <b>Warning</b> : input contains tricky cases too.</p>

<p>A single line of human-readable-Python code can get AC in the third of the time limit. A fast C code ends in 0.04s. (edit 2017-02-11, after compiler changes)<br>
;-) Have fun.</p>