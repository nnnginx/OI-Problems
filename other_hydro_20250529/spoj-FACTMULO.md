<p>For <strong><em>n</em></strong> positive integer, let <strong><em>F(n) = 1! ¡Á 2! ¡Á 3! ¡Á 4! ¡Á ... ¡Á n!</em></strong>, product of factorial(i) for i in [1..n],<br>


<br>

For <strong><em>p</em></strong> a prime number, and <strong><em>n</em></strong> an integer,
and let <strong><em>V(p, n) = max({i&gt;=0 integer, such that p^i divides F(n)})</em></strong>. <br>




</p><h3>Input</h3>
<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.<br>
On each of the next <strong><em>T</em></strong> lines, your are given
two integers <strong><em>p</em></strong> a prime number, and <strong><em>n</em></strong>.
</p>

<h3>Output</h3>
<p>For each test case, you have to print <strong><em>V(p, n)</em></strong>.
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
2 3
3 4
</pre>
<pre><strong>Output:</strong>
2
2
</pre>

<h3>Constraints</h3>
<pre>0 &lt; T &lt; 10^5
1 &lt; p &lt; 10^18, a prime number
0 &lt; n &lt; 10^18
</pre>
<p><strong><em>p</em></strong> and <strong><em>n</em></strong> are log-uniform independent randomly distributed.</p>

<p>Four lines of Python code can get AC in half the time limit. (Edit 2017-02-11, after compiler changes)<br>
;-) Have fun.</p>