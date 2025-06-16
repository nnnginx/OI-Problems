<p>Factorize <em>x<sup>n</sup>-1</em> into several irreducible polynomials over the integers.</p>
<h3>Input</h3>
<p>Multiply test cases. For each test case:</p>
<p>A single line - <em>n</em>.(2&lt;= <em>n</em> &lt;= 1200).</p>
<p>Input terminates by a single zero.</p>
<h3>Output</h3>
<p>For each test case, output the factorization of the given polynomial.</p>
<p>There are multiple ways to express the factorization of a polynomial. To make it unique, we sort the irreducible polynomials according to the following rules:</p>
<p>Lower order polynomials are always lexicographically smaller than higher order polynomials. Same order polynomials should be sorted by their coefficients. We compare the coefficients from high degree terms to low degree terms, including the omitted terms, which the coefficients are regard as 0. Coefficients are being compared first by absolute value then by sign. Smaller absolute values are lexicographically smaller. For the same absolute value, negative coefficients are lexicographically smaller than positive coefficients.</p>
<p>See example for more output format details.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
12
0

<strong>Output:</strong>
(x-1)(x+1)(x^2+1)(x^2-x+1)(x^2+x+1)(x^4-x^2+1)
</pre>
<h3>Hint</h3>
<p>There should <b>not</b> be a "*" between digit and x, i.e. -2x^2 should be printed as -2x^2.</p>