<p align="justify">Your task consists of evaluate a polynomial of degree <strong>n</strong> (<strong>0</strong> &lt;= <strong>n</strong> &lt;= <strong>999</strong>) represented by its <strong>n+1</strong> coefficients of the form:
 </p>
 
<center>
  <strong>p<sub>n</sub>(x)  = c<sub>n</sub>x<sup>n</sup> + c<sub>n-1</sub>x<sup>n-1</sup> + бн + c<sub>2</sub>x<sup>2</sup> + c<sub>1</sub>x + c<sub>0</sub></strong>
</center>
<p align="justify">in each one of the <strong>k</strong> (<strong>1</strong> &lt;= <strong>k</strong> &lt;= <strong>100</strong>) points <strong>x<sub>1</sub></strong>, <strong>x<sub>2</sub></strong>,  бн, <strong>x<sub>k</sub></strong>. The coefficients of the polynomial and the values where they will be evaluated are integers in the interval <strong>[-100, 100]</strong> that guarantees that the polynomial's evaluation is at the most <strong>2<sup>63</sup> иC 1</strong>.
</p>

<h3>Input</h3>
<p align="justify">
There will be multiple test cases, each one with <strong> 4</strong> lines that are described below
<br>
<b>n</b>: degree of polynomial.<br>

<strong>c<sub>n</sub> c<sub>n-1 </sub>бн  c<sub>2 </sub> c<sub>1</sub>  c<sub>0</sub></strong>: coefficients of the polynomial separated by a single space.<br>

<strong>k</strong>: number of points to evaluate the polynomial.<br>

<strong>x<sub>1</sub> x<sub>2 </sub>бн<sub> </sub> x<sub>k-1</sub> x<sub>k</sub></strong>: points to evaluate the polynomial separated by a single space.<br>
<br>
The final test case is a single line where <strong>n = -1</strong> and this case should not be processed.
</p>

<h3>Output</h3>
<p align="justify">
For each test case you should print <strong>k + 1</strong> lines of output, the very first line containing the case number and the following <strong>k</strong> lines with the result of the polynomial's evaluation in each one of the <strong>k</strong> given points. See the sample.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
2<br>1 -2 -1<br>5<br>0 1 -1 2 -2<br>3<br>2 1 -2 -1<br>4<br>0 -1 2 -2<br>-1<br>
<b>Output:</b>
Case 1:<br>-1<br>-2<br>2<br>-1<br>7<br>Case 2:<br>-1<br>0<br>15<br>-9<br>
</pre>