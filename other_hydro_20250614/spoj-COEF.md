<p>The problem is to calculate the coefficients in expansion of polynomial <em>(x<sub>1</sub>+x<sub>2</sub>+...+x<sub>k</sub>)<sup>n</sup></em>.</p>

<h3>Input</h3>
<p>The input will consist of a set of pairs of lines. The first line of the  pair consists of two integers <em>n</em> and <em>k</em> separated with space (<em>0 &lt; n, k &lt;13</em>). This integers define the power of the polynomial and the amount of the variables. The second line in each pair consists of <em>k</em> non-negative integers <em>n<sub>1</sub>, ...,  n<sub>k</sub>,</em> where <em>n<sub>1</sub>+...+n<sub>k</sub>=n</em>.</p>

<h3>Output</h3>
<p>For each input pair of lines the output line should consist one integer,  the coefficient by the monomial <em>x<sub>1</sub><sup>n1</sup>x<sub>2</sub><sup>n2</sup>...x<sub>k</sub><sup>nk</sup></em> in expansion of the polynomial <em>(x<sub>1</sub>+x<sub>2</sub>+...+x<sub>k</sub>)<sup>n</sup></em>.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
2 2
1 1
2 12
1 0 0 0 0 0 0 0 0 0 1 0

<strong>Output:</strong>
2
2</pre>