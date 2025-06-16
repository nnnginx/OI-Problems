<p style="text-align: center;"><img title="pwsum" src="../../../content/syntax_error:pwsum.png" alt="suma" width="82" height="112"></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Everyone knows that we can express sums of form sigma i = 1 to x ( i^k ) as polynomials</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">of degree k+1. Most people find it hard to derive actual formulas for such sums, so</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">we'd like to have a program that does that for us! You are given a nonnegative</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">integer K, and you're asked to compute the coefficient representation of the polynomial</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">which defines the sum shown above. However, we'd like to simplify your computation</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">so you only have to output the formula modulo 10007. ( A formula which correctly computes</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">the remainder of the sum when divided by 10007, for any natural x ).</div>
<p>Everyone knows that we can express sums this form as polynomials&nbsp;of degree k+1. Most people find it hard to derive actual formulas for such sums, so&nbsp;we'd like to have a program that does that for us! You are given a nonnegative&nbsp;integer K, and you're asked to compute the coefficient representation of the polynomial&nbsp;which defines the sum shown above. However, we'd like to simplify your computation&nbsp;so you only have to output the formula modulo 10007. ( A formula which correctly computes&nbsp;the remainder of the sum when divided by 10007, for any natural x ).</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first and only line of input contains a nonnegative integer k ( 0 &lt;= k &lt;= 300 ): the power we use&nbsp;in our sum.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>The first and only line of output should contain the canonic coefficient representation of the&nbsp;formula. To elaborate, this should be the form of your output:</p>
<p>a<sub>k+1</sub>x<sup>k+1</sup> + a<sub>k</sub>x<sup>k</sup> + a<sub>k-1</sub>x<sup>k-1</sup> ... a<sub>0</sub>x<sup>0</sup></p>
<p>ai here represents the coefficient that stands by the i-th power of x.&nbsp;As we only wish to find the formula modulo 10007, all the coefficients should be&nbsp;from interval [0, 10006] of integers. See the sample input and output for further clarification.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><strong><span style="font-weight: normal; ">1</span></strong>

<strong>Output:</strong>
</pre>
<pre>5004x^2 + 5004x^1 + 0x^0</pre>
<pre><strong><br></strong></pre>
<pre><strong>Input:</strong></pre>
<pre>3</pre>
<pre><strong>Output:</strong></pre>
<pre>2502x^4 + 5004x^3 + 2502x^2 + 0x^1 + 0x^0</pre>
<div style="text-align: left;"><strong><br></strong></div>