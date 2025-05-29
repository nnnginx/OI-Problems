<p>
After solving <a href="http://www.spoj.com/problems/BMS1988/">Fib-Factorization</a> and <a href="http://www.spoj.com/problems/PISANO/">ModFib-Period</a>, you would probably be interested by solving this new task:<br>
Simply compute Fib(N) mod Fib(K), where Fib(N) denotes the Nth term of the Fibonacci sequence.<br>
(If N&lt;2 Fib(N)=N, else Fib(N)=Fib(N-1)+F(N-2)).
</p>

<h3>Input</h3>
<p>
The input begins with the number T of test cases in a single line.<br>
In each of the next T lines there are two integers N, K.
</p>


<h3>Output</h3>
<p>
For each test case, on a single line, print Fib(N) mod Fib(K).
</p>


<h3>Example</h3>
<pre><b>Input:</b>
2
5 5
13 5


<b>Output:</b>
0
3
</pre>

<h3>Constraints</h3>
<pre>1 &lt; T &lt; 10^5
1 &lt; N &lt; 10^18
1 &lt; K &lt;= 10^3
</pre>
<p>Edit(2017-02-11) : New time limit (after compiler changes).
</p>