<h3>Input</h3>
<p>Multiple test cases. For each test case:</p>
<p>The first line contains integers N and M; N is a number of nodes in the circuit (2 &lt; N &lt;= 100), M is the number of resistors (0 &lt;= M &lt;= 300). Each of the next M lines consists of three integers A<sub>i</sub>, B<sub>i</sub> and R<sub>i</sub> ¡ª description of a resistor that has resistance R<sub>i</sub> connecting the nodes A<sub>i</sub> and B<sub>i</sub> (1 &lt;= A<sub>i</sub> , B<sub>i</sub> &lt;= N; 1 &lt;= R<sub>i</sub> &lt;= 100).</p>
<p>There's a blank line between consecutive test cases in the input file. No other extra whitespace will/should be appear in the input/output.</p>
<p>Input terminates by EOF.</p>
<h3>Output</h3>
<p>For each test case, output the total resistance between the nodes 1 and N rounded within two digits after a decimal points. There won't be any test case the output for which is +INF. </p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 5
1 2 15
2 4 5
1 3 10
3 4 10
2 3 1

<strong>Output:</strong>
9.40
</pre>