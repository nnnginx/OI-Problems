<p>You are given the polynomial F(x) as the sum of monomials.
Each monomial has the form: <br>[<i>coefficient</i>*]<i>x</i>[^<i>degree</i>] or [<i>coefficient</i>],<br>
where <i>coefficient</i> and <i>degree</i> are integers such that -30000 &lt;= <i>coefficient</i> &lt;= 30000, 0 &lt;= <i>degree</i> &lt;= 6. The parameters given in [] can be skipped.<br>
In this problem you have to find all solutions of the equation: F(x)=0.</p>

<h3>Input</h3>
<p><i>t</i> ¨C the number of test cases, then <i>t</i> test cases follow. [<i>t</i> &lt;= 100]<br>
Each line contains one polynomial <i>F(x)</i> given as string <i>s</i> in the form described above.<br>
The length of string <i>s</i> is not more than 300 characters.

</p><h3>Output</h3>
<p>For each test case output all solutions (including repeated) of the given equation in non-decreasing order. All solutions lie within the interval [-100.0; 100.0]. Each solution must be given with an error of not more than 0.01. It's guaranteed that all solutions are real, not complex.

</p><h3>Example</h3>
<pre><b>Input:</b>
2
x^4-6*x^3+11*x^2-6*x
-x^2+2*x-1

<b>Output:</b>
0.00 1.00 2.00 3.00
1.00 1.00
</pre>