<p>There's a 5¡ÁN rectangular corridor in the hall's dojo, one place is already taken by a magic hanj¨­ (1¡Á1 square).
You have to put tatamis (1¡Á2 rectangle) in order to cover exactly the rest of the corridor.
Sometimes it's possible, sometimes not!
</p>

<h3>Input</h3>
<p>The input begins with the number T of test cases in a single line.
In each of the next T lines there are an integer N the H-length of the corridor,
and I, J the coordinates of the magic hanj¨­. See sample input for details format.
</p>

<h3>Output</h3>
<p>For each test case, print the number of possibility to do the job, modulo 1000000007.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
1 C 1
3 B 2
5 A 1

<b>Output:</b>
1
8
192
</pre>
<p><img title="Corridor" src="../../content/francky:doj2-fig" alt="Corridor"></p>

<h3>Constraints</h3>
<p>1 &lt;= T &lt;= 40 000</p>
<p>1 &lt;= N &lt;= 20 000</p>
<p>A &lt;= I &lt;= E</p>
<p>1 &lt;= J &lt;= N</p>

<p>Uniform, independent, random input in the range. Input had been 'filtered' to let only possible configurations.</p>

<p>You may try too : <a href="../../problems/BTCODE_J/">Grid Tiling</a>, or <a href="../../problems/PBOARD/">Blocks for kids</a> </p>
<p>Edit(19/I/2015, after cluster switch) : now my old code ends in 0.23s using PY3.4.</p>
<p>Edit(11-2-2017, after compiler update) : now my old code ends in 0.10s using PY3.5. New TL.</p>