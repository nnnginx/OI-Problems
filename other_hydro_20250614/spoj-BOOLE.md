<p>

Propositions are logical formulas consisting of proposition symbols and connecting operators.
They are recursively defined by the following rules:

</p><ol>
<li>All proposition symbols (in this problem, lower-case alphabetic characters, e.g., <code>a</code> and <code>z</code>) are propositions.

</li><li>If <code>P</code> is a proposition, <code>(!</code><code>P</code><code>)</code> is a proposition, and <code>P</code> is a direct subformula of it.
</li><li>If <code>P</code> and <code>Q</code> are propositions, <code>(</code><code>P</code><code>&amp;</code><code>Q</code><code>)</code>, <code>(</code><code>P</code><code>|</code><code>Q</code><code>)</code>, <code>(</code><code>P</code><code>--&gt;</code><code>Q</code><code>)</code>, and <code>(</code><code>P</code><code>&lt;-&gt;</code><code>Q</code><code>)</code> are propositions, and <code>P</code> and <code>Q</code> are direct subformulas of them.

</li><li>Nothing else is a proposition.
</li></ol>

The operations <code>!</code>, <code>&amp;</code>, <code>|</code>, <code>--&gt;</code>, and <code>&lt;-&gt;</code> denote logical negation, conjunction, disjunction, implication, and equivalence, respectively.
A proposition <code>P</code> is a subformula of a proposition <code>R</code> if <code>P=R</code> or <code>P</code> is a direct subformula of a proposition <code>Q</code> and <code>Q</code> is a subformula of <code>R</code>.


<p>

Let <code>P</code> be a proposition and assign boolean values (i.e., <code>0</code> or <code>1</code>) to all proposition symbols that occur in <code>P</code>.
This induces a boolean value to all subformulas of <code>P</code> according to the standard semantics of the logical operators:

</p><p>

</p><center>
<table border="">
<tbody><tr>
<td>negation
</td><td>conjunction
</td><td>disjunction
</td><td>implication
</td><td>equivalence
</td></tr><tr>
<td><code>!</code><code>0</code>=<code>1</code>
</td><td><code>0</code><code>&amp;</code><code>0</code>=<code>0</code>

</td><td><code>0</code><code>|</code><code>0</code>=<code>0</code>
</td><td><code>0</code><code>--&gt;</code><code>0</code>=<code>1</code>
</td><td><code>0</code><code>&lt;-&gt;</code><code>0</code>=<code>1</code>

</td></tr><tr>
<td><code>!</code><code>1</code>=<code>0</code>
</td><td><code>0</code><code>&amp;</code><code>1</code>=<code>0</code>
</td><td><code>0</code><code>|</code><code>1</code>=<code>1</code>

</td><td><code>0</code><code>--&gt;</code><code>1</code>=<code>1</code>
</td><td><code>0</code><code>&lt;-&gt;</code><code>1</code>=<code>0</code>
</td></tr><tr>
<td>
</td><td><code>1</code><code>&amp;</code><code>0</code>=<code>0</code>

</td><td><code>1</code><code>|</code><code>0</code>=<code>1</code>
</td><td><code>1</code><code>--&gt;</code><code>0</code>=<code>0</code>
</td><td><code>1</code><code>&lt;-&gt;</code><code>0</code>=<code>0</code>

</td></tr><tr>
<td>
</td><td><code>1</code><code>&amp;</code><code>1</code>=<code>1</code>
</td><td><code>1</code><code>|</code><code>1</code>=<code>1</code>
</td><td><code>1</code><code>--&gt;</code><code>1</code>=<code>1</code>

</td><td><code>1</code><code>&lt;-&gt;</code><code>1</code>=<code>1</code>
</td></tr></tbody></table>
</center>

<p>

This way, a value for <code>P</code> can be calculated.
This value depends on the choice of the assignment of boolean values to the proposition symbols.
If <code>P</code> contains <code>n</code> different proposition symbols, there are <code>2<sup>n</sup></code> different assignments.
To evaluate all possible assignments we may use truth tables.


</p><p>

A truth table contains one line per assignment (i.e., <code>2<sup>n</sup></code> lines in total).
Every line contains the values of all subformulas under the chosen assignment.
The value of a subformula is aligned with the proposition symbol, if the subformula is a proposition symbol, and with the center of the operator otherwise.

</p><h3>Input Specification</h3>
<p>

The input contains several test cases, each on a separate line.
Every test case denotes a proposition and may contain arbitrary amounts of spaces in between.
The input file terminates immediately after the newline symbol following the last test case.

</p><h3>Output Specification</h3>
<p>

For each test case generate a truth table for the denoted proposition.
Start the truth table by repeating the input line.
Evaluate the proposition (and its subformulas) for all assignments to its variables, and output one line for each assignment.
The line must have the same length as the corresponding input line and must consist only of spaces and the characters <code>0</code> and <code>1</code>.
Output an empty line after each test case.


</p><p>

Let <code>s<sub>1</sub>,...,s<sub>n</sub></code> be the proposition symbols in the denoted proposition sorted in alphabetic order.
Then, all assignments of <code>0</code> to <code>s<sub>1</sub></code> must precede the assignments of <code>1</code> to <code>s<sub>1</sub></code>.
Within each of these blocks of assignments, all assignments of <code>0</code> to <code>s<sub>2</sub></code> must precede the assignments of <code>1</code> to <code>s<sub>2</sub></code>, and so on.


</p><h3>Sample Input</h3>
<p>

</p><pre>((b --&gt; a) &lt;-&gt; ((! a) --&gt; (! b)))
  ((y &amp;  a)   -  -&gt;(c |c))
</pre>

<h3>Sample Output</h3>
<p>

</p><pre>((b --&gt; a) &lt;-&gt; ((! a) --&gt; (! b)))
  0  1  0   1    1 0   1   1 0   
  1  0  0   1    1 0   0   0 1   
  0  1  1   1    0 1   1   1 0   
  1  1  1   1    0 1   1   0 1   

  ((y &amp;  a)   -  -&gt;(c |c))
    0 0  0       1  0 00  
    1 0  0       1  0 00  
    0 0  0       1  1 11  
    1 0  0       1  1 11  
    0 0  1       1  0 00  
    1 1  1       0  0 00  
    0 0  1       1  1 11  
    1 1  1       1  1 11  

</pre>