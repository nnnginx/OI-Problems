<p align="justify">
Transform the algebraic expression with brackets into RPN form (Reverse Polish Notation). Two-argument operators: +, -, *, /, ^ (priority from the lowest to the highest), brackets ( ). Operands: only letters: a,b,...,z. Assume that there is only one RPN form (no expressions like a*b*c).
</p>
<h3>Input</h3>
<pre><i>t</i> [the number of expressions &lt;= <b>100</b>]
<i>expression</i> [length &lt;= <b>400</b>]
[other expressions]
</pre>
<p align="left">
Text grouped in [ ] does not appear in the input file.
</p>
<h3>Output</h3>
<pre>The <em>expression</em>s in RPN form, one per line.
</pre>
<h3>Example</h3>
<pre>Input:
3
(a+(b*c))
((a+b)*(z+x))
((a+t)*((b+(a+c))^(c+d)))

Output:
abc*+
ab+zx+*
at+bac++cd+^*</pre>