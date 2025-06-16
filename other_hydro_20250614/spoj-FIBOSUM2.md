<p>
Some people may found <a href="http://www.spoj.com/problems/FIBOSUM/">FIBOSUM</a> a too easy problem.
We propose here a useful variation.</p>

<img title="SigmaFibScale" src="../../content/francky:sigmaFibScale" alt="SigmaFibScale">
<p>
Fib is the Fibonacci sequence:<br>
For any positive integer i: if i&lt;2 Fib(i) = i, else Fib(i) = Fib(i-1) + Fib(i-2)
</p>
<h3>Input</h3>
<p>The first line of input contains an integer
 <strong><em>T</em></strong>, the number of test cases.<br>
On each of the next <strong><em>T</em></strong> lines, your are given
tree integers <strong><em>c</em></strong>, <strong><em>k</em></strong>, <strong><em>N</em></strong>.
</p>

<h3>Output</h3>
<p>
Print <strong>Sum(Fib(<em>ki+c</em>) for <em>i</em> in [1..<em>N</em>])</strong>.
<br>
As the answer could not fit in a 64-bit container, just output your answer modulo 1000000007.
</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1
3 5 2
</pre>
<pre><strong>Output:</strong>
254
</pre>
<h3>Explanations</h3>
<p>
Index-1 Fib sequence : 1, 1, 2, 3, 5, 8, 13, <b>21</b>, 34, 55, 89, 144, <b>233</b>, 377, 610, 987, ...<br>
We want the 5*1+3 = 8<sup>th</sup> and 5*2+3 = 13<sup>th</sup> ones, thus the answer is 21 + 233 = 254.
</p>

<h3>Constraints</h3>
<pre>0 &lt; T &lt;= 60606
0 &lt;= c &lt; k &lt;= 2^15
0 &lt; N &lt;= 10^18
</pre>
<p>
The numbers <strong><em>c,k,N</em></strong> are uniform randomly chosen in their range.
<br>
For your information, constraints allow 1.3kB of Python3 code to get AC in 6.66s, it could be hard.<br>
A fast C-code can get AC under 0.15s.<br>
<b>Warning:</b> Here is Pyramid cluster, you can try the <a href="http://www.spoj.com/problems/FIBOSUMT/">tutorial edition</a> (clone with Cube cluster).<br>
<strong>Have fun ;-)</strong>
</p>
<p>
Edit(2017-02-11) : With compiler changes, my fast C code ends in 0.01s, my Python3 ones in 0.31s. New TL is 0.5s.
</p>