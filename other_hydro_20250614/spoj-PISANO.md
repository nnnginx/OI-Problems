<p>
Perhaps the first thing one notices when the Fibonacci sequence is reduced mod M is that
it seems periodic.</p>

<p>
For example :<br>
F (mod 4) = <b>0 1 1 2 3 1</b> 0 1 1 2 3 ... <br>
F (mod 5) = <b>0 1 1 2 3 0 3 3 1 4 0 4 4 3 2 0 2 2 4 1</b> 0 1 1 2 3 ... <br>
</p>

<p>
We define K(M) the period of the Fibonacci sequence reduced mod M if it is periodic.<br>
We just saw that K(4) = 6 and K(5) = 20.
</p>

<h3>Input</h3>
<p>
The input begins with the number T of test cases in a single line.<br>
In each of the next T lines there are one integer M.
</p>


<h3>Output</h3>
<p>
For each test case, on a single line, print K(M), or "Not periodic." without quotes if need.
</p>

<h3>Example</h3>
<pre><b>Input:</b>
3
4
5
6

<b>Output:</b>
6
20
24
</pre>

<h3>Constraints</h3>
<pre>1 &lt; T &lt; 10^4
1 &lt; M &lt; 10^12
</pre>
<p>
Edit 2017-02-11, after compiler changes ; new TL. My old Python code end in 1.92s.
</p>