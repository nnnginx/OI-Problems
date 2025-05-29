<p>Leo would like to play with some really big numbers, OK...</p>

<p>Let  FIB  the Fibonacci function :<br>
  FIB(0)=0 ; FIB(1)=1<br>
  and<br>
  for N&gt;=2  FIB(N) = FIB(N-1) + FIB(N-2)<br>
<br>
Example : we have FIB(6)=8, and FIB(8)=21, so FIB(FIB(6))=21
</p>

<h3>Input</h3>
<p>The input begins with the number T of test cases in a single line.<br>
In each of the next T lines there are an integer N.
</p>

<h3>Output</h3>
<p>For each test case, print  FIB(FIB(N)) ,<br>
as the answer could not fit in a 64bit container,<br>
give your answer modulo 1000000007.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
0
5
6

<b>Output:</b>
0
5
21
</pre>



<h3>Constraints</h3>
<pre>1 &lt;= T &lt;= 10^4
0 &lt;= N &lt;= 10^100
</pre>
<p>Time limit is set to allow (sub-optimal) 500B of python3 code to get AC.<br>
A near optimal solution is within 0.02 and 0.04s with a fast language, and around 1s in Python2 without psyco. </p>
<p>Edit(20/I/2015) With Cube cluster, it is not hard to get 0.0s with fast languages, and my old code ended in 0.08s using PY3.4.</p>
<p>Edit(11-2-2017) With compiler update, new TL. My old Python code ends in 0.04s, and it's easy to get 0.00s using a fast language.</p>