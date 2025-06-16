<p> Ileana D'Cruz is taking programming classes but she is having problem in understanding <b>while loops</b>. She is working on following set of instructions -<br>
</p><p><font color="BLUE">INTEGER</font> <b> I = 0, S, U = 10<sup>10</sup></b>;<br>
</p><p><font color="BLUE"><b>WHILE</b></font> (I &lt; U) <font color="RED"><b>{</b></font><br>
    S = (3 * S) + (5 * I);<br>
    I = I + 1;<br>
<font color="RED"><b>}</b></font><br>
</p><p>Let <b>S<sub>k</sub></b> be the value assigned to INTEGER <b>S</b> for the iteration <b>I = (k + 1)</b> and <b>n, m, p</b> be positive integers such that <b>m &gt; n.</b> Ileana knows the values of <b>n</b> and <b>m</b> but she forgot the initial value of <b>S</b>. She is trying to find the unit digit of <b>p</b>. Any initial value of S may be used. She also knows the following equality -<br>
</p><p><b><font color="BLUE">(2 * n + 3) * (p - 1)</font> <b>+</b><font color="RED"> (4 / 5) * [(p * S<sub>n</sub>) - S<sub>m</sub>]</font> <b>=</b><font color="BLUE"> 2 * (m - n)</font></b><br> 
</p><h3>Input</h3>
<p>First line of input is <b>T</b>(total no. of test cases). Each of next T lines contains two integers <b>n</b> and <b>m</b>.

</p><h3>Output</h3>
<p>Print <b>unit digit of p (p % 10) </b> for each test case in separated lines.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
2 3

<b>Output:</b>
3
</pre>

<h3>Constraints</h3>
<p><b>T &lt; 10001</b><br>

</p><h3>Explanation</h3>
<p>Let S = 2<br>
S<sub>0</sub> = 6<br>
S<sub>1</sub> = 23<br>
S<sub>2</sub> = 79<br>
S<sub>3</sub> = 252<br>
Now solving the equation gives <b>p = 3</b>.
</p>