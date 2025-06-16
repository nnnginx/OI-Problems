<p>There's a long rectangular corridor in the hall's dojo, one place is already taken by a magic hanj¨­ (1¡Á1 square). You have to put tatamis (1¡Á2 rectangle) in order to cover exactly the rest of the corridor. Sometimes it's possible, sometimes not!</p>
<h3>Input</h3>
<p>The input begins with the number T of test cases in a single line. In each of the next T lines there are two integers : N, M the size of the corridor, I,J coordinates of the magic hanj¨­, and K the modulo for the output.</p>
<h3>Output</h3>
<p>For each test case, print the number of possibility to do the job, modulo K.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
1 3 1 3 100
2 3 2 2 100
3 7 1 3 100

<strong>Output:</strong>
1
0
56
</pre>
<p><img title="Corridor" src="../../content/francky:doj1-fig" alt="Corridor"></p>
<h3>Constraints</h3>
<p>1 &lt;= T &lt;= 30000</p>
<p>1 &lt;= N &lt;= 4</p>
<p>1 &lt;= M &lt;= 10^9</p>
<p>1 &lt;= I &lt;= N</p>
<p>1 &lt;= J &lt;= M</p>
<p>1 &lt;= K &lt;= 10^9</p>
<p>Uniform, independent, random input in the range.</p>
<p>Time limit is set to allow one half kB of python3 code to get AC.</p>
<p>Edit(19/I/2015, after cluster switch) : now my old code ends in 0.16s using PY3.4.</p>
<p>Edit(11-2-2017, after compiler update) : new TL. My old code ends in 0.09s using PY3.5.</p>