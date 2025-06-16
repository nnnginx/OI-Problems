<p>
Perhaps the first thing one notices when the Fibonacci sequence is reduced mod <em>p</em> is that
it seems periodic.</p>

<p>
For example :<br>
F (mod 2) = <b><u>0</u> 1 1</b> 0 1 1 0 1 ... <br>
F (mod 3) = <b><u>0</u> 1 1 2 <u>0</u> 2 2 1</b> 0 1 1 2 ... <br>
F (mod 5) = <b><u>0</u> 1 1 2 3 <u>0</u> 3 3 1 4 <u>0</u> 4 4 3 2 <u>0</u> 2 2 4 1</b> 0 1 1 2 3 ... <br>
</p>

<p>
We define <em>Z</em>(<em>p</em>) the number of zeros in fundamental period of Fibonacci numbers mod <em>p</em> (if it is periodic).<br>
We just saw that <em>Z</em>(2) = 1, <em>Z</em>(3) = 2, and <em>Z</em>(5) = 4.
</p>

<h3>Input</h3>
<p>
The first line contains <em>T</em>, the number of test cases.<br>
Each of the next <em>T</em> lines contains a prime number <em>p</em>.
</p>


<h3>Output</h3>
<p>
For each test case, print <em>Z</em>(<em>p</em>), or "Not periodic." without quotes if need.
</p>

<h3>Example</h3>
<pre><b>Input:</b>
3
2
3
5

<b>Output:</b>
1
2
4
</pre>

<h3>Constraints</h3>
<pre>1 &lt; T &lt; 10^5
1 &lt; p &lt; 10^18, a prime number
</pre>
<p>There's two input files, in the first one you are given all primes under 10^6, in the second one lot of uniform randomly chosen primes.<br>
<strong>Warning</strong> : Time limit had been changed, and could not allows slow languages to get AC here. This problem allows easy coding using languages without bigNum library, but you need to be able to get at least some few points at <a href="http://www.spoj.com/problems/FIB64/">FIB64</a>.<br>
My best C-timing is 0.12s. (Edit : 0.03s with cluster change)<br>
For other languages, take a look at <a href="http://www.spoj.com/problems/Z124H/">Z124H</a> with higher constraints.
<strong>Good luck, and have fun ;-)</strong><br>
</p>