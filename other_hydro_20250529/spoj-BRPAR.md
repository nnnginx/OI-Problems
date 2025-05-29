<p>Count the number of different correct bracket sequences consisting of k1 pairs of brackets of the 1st type, k2 pairs of brackets of the 2nd type, бн, km pairs of brackets of the m-th type. The bracket sequence is considered correct in the following cases:</p><ul><li>empty sequence is correct;</li><li>if A is correct and B is correct then AB is correct;</li><li>if A is correct then (<sub>i</sub>A)<sub>i</sub> is correct where (<sub>i</sub> and )<sub>i</sub> are opening and closing brackets of the same type.</li></ul><p></p>


<h3>Input</h3>
<p>The first line of input is the number 0 &lt; n &lt;= 1000 of test cases. Each of the following n lines describe a test case. Each line starts with number 0 &lt; m &lt;= 100 the amount of different bracket types. Then m positive numbers k1, k2, бн, km follow each separated with a space. Number ki is the amount of pairs of brackets of i-th type. The total amount of pairs of brackets is not greater than 1000.</p>

<h3>Output</h3>
<p>For each test case output a line containing single integer иC the answer to the problem modulo 1000000007.</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
1 4
2 2 2
3 1 2 3

<b>Output:</b>
14
84
7920
</pre>