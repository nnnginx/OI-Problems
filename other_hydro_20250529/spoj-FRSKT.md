<p>Let  FIB  the Fibonacci function :<br>
  FIB(0)=0 ; FIB(1)=1<br>
  and<br>
  for N&gt;=2  FIB(N) = FIB(N-1) + FIB(N-2)<br>
</p>

<p>Example : we have FIB(6)=8, and FIB(8)=21.</p>

<p> </p>

<p>Let F(K, N) a new function: <br>
F(0, N) = N for all integers N.<br>
F(K, N) = F(K-1, FIB(N) ) for K&gt;0 and all integers N.</p>

<p>Example : F(2, 6) = F(1, FIB(6) ) = F(0, FIB( FIB(6) ) ) = FIB( FIB(6) ) = FIB(8) = 21</p>


<h3>Input</h3>
<p>The input begins with the number T of test cases in a single line.<br>
In each of the next T lines there are three integers: K, N, M.
</p>

<h3>Output</h3>
<p>For each test case, print F(K, N),<br>
as the answer could not fit in a 64bit container,<br>
give your answer modulo M.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
4 5 1000
3 4 1000
2 6 1000

<b>Output:</b>
5
1
21
</pre>

<h3>Constraints</h3>

<pre>1 &lt;= T &lt;= 10^3
0 &lt;= K &lt;= 10^2
0 &lt;= N &lt;= 10^9
2 &lt;= M &lt;= 10^9
</pre>

<p>You would perhaps have a look, after, at the <a href="http://www.spoj.com/problems/FRSKH/">hard edition</a> with more difficult constraints.</p>
<p>Edit 2017-02-11, after compiler update. My old Python code ends in 0.08s. New TL.</p>