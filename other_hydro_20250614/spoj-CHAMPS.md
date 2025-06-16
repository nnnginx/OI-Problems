<p align="justify">&nbsp;</p>
<p>Michel is participating in a championship where each participant have p<sub>i</sub> (0&lt;=i&lt;=N-1) points. He knows for some pairs of participants an inequality between the points of each one, in the form p<sub>A</sub> -p<sub>B</sub> &gt;= C. Now he wants to know if his data is correct, i.e., if its possible to assign points for each participant and satisfy all the inequalities.</p>
<h3>Input</h3>
<p>The input consists of several test cases (at most 150). The first line of each test case consists of two integers N and M (1&lt;=N&lt;=500, 0&lt;=M&lt;=5000). Then follow M lines of three integers A, B and C, indicating that p<sub>A</sub> -p<sub>B</sub> &gt;= C (0&lt;=A,B&lt;=N-1, |C|&lt;=20000).</p>
<h3>Output</h3>
<p>Print a single line for each test case with 'y' if the data is valid or 'n' if its not.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input</strong>
2 2
0 1 2
1 0 2
4 4
0 1 1
1 2 1
2 3 -2
3 0 1
4 4
0 1 1
1 2 1
2 3 -3
3 0 1

<strong>Output</strong>
n
n
y

</pre>