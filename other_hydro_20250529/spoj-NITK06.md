<p>Suppose we have a sequence of non-negative integers, Namely a<sub>1</sub>, a<sub>2</sub>,  ..., a<sub>n</sub>. 
At each time we can choose one term a<sub>i</sub> with 0 &lt; i &lt; n  and we subtract 1 from both a<sub>i</sub> and a<sub>i+1</sub>. 
We wonder whether we can get a  sequence of all zeros after several operations.</p>

<h3>Input</h3>
<p>The first line is the number of test cases T (0 &lt; T &lt;= 20).</p>
<p>The first line of each test case is a number N (0 &lt; N &lt;= 10000). The next line is N non-negative integers, 0 &lt;= a<sub>i</sub> &lt;= 10<sup>9</sup>.</p>

<h3>Output</h3>
<p>If it can be modified into all zeros with several operations output <tt>¡°YES¡±</tt> in a single line, otherwise output <tt>¡°NO¡±</tt> instead.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2
2
1 2
2
2 2

<strong>Output:</strong>
NO
YES</pre>

<h3>Explanation</h3>
<p>It is clear that [1 2] can be reduced to [0 1] but no further to convert all integers to 0. Hence, the output is NO.</p>
<p>In second case, output is YES as [2 2] can be reduced to [1 1] and then to [0 0] in just two steps.</p>