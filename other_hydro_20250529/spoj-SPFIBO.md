<p>Fibonacci sequence is defined as follow: F<sub>1</sub> = 1, F<sub>2</sub> = 2, F<sub>i</sub> = F<sub>i-1</sub> + F<sub>i-2</sub> (i &gt; 2).</p>
<p>Each natural number X can be expressed by the maximum numbers that are less than or equal to X in Fibonacci sequence: X = a<sub>1</sub>xF<sub>1</sub> + a<sub>2</sub>xF<sub>2</sub> + ¡­ Therefore, in Fibonacci system, X is known as: a<sub>n</sub>a<sub>n-1</sub>¡­a<sub>1</sub>. For example, 1 = 1<sub>F</sub>, 2 = 10<sub>F</sub>, etc. If we write all natural numbers successively in Fibonacci system, we will obtain a sequence like this: 1_1_0¡­ This is called ¡°Fibonacci bit sequence of natural numbers¡±.</p>
<p>Your task is counting the numbers of times that bit 1 appears in the first N bits of this sequence.</p>
<h3>Input</h3>
<p>Line 1: An integer N (1 &lt;= N &lt;= 10<sup>15</sup>)</p>
<h3>Output</h3>
<p>Line 1: An integer K is the result</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br><br><strong>Output:</strong><br>2<br></pre>