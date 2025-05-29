<p>Consider a  10x10  grid. Cells in this grid can contain one of
five logic operations (AND, OR, NOT,
Input, Output). These can be joined together to form a logic circuit.
Given a description of a circuit
and a set of boolean values, build the logic circuit and execute the input
stream against it.
</p><p>
</p><h3>Input</h3>
<p>The first line of the input contains a single integer <i>n</i>, which specifies the number of circuits to be
processed. There will then be <i>n</i> groups of circuit descriptions and test values.
</p><p>
</p><p>
A circuit is made up of a number of operations. Each line describing an operation begins with three
characters: the co-ordinates for a cell, 0-9 on the <i>X</i>-axis then 0-9 on the <i>Y</i>-axis, followed by a single
character to represent the operation of that cell (`<tt>&amp;</tt>' for AND, `<tt>|</tt>' for OR,
`<tt>!</tt>' for NOT, `<tt>i</tt>' for Input and `<tt>o</tt>'
for Output). Optionally following each triple is a set of co-ordinate
pairs which represent the <i>x</i> and <i>y</i>

co-ordinates of cells that take the output of this cells operation as an input for theirs. This (possibly
empty) output list is terminated by `<tt>..</tt>'. The list of operations is terminated by a line containing the
word `<tt>end</tt>'.
</p>
<p>
Next, for each circuit, comes the set of test values. The first line contains
an integer <i>t</i> which gives the number of test cases your program must run. Next, there are <i>t</i> lines, each line containing a
sequence of `<tt>0</tt>' and `<tt>1</tt>' characters symbolising the input values for one test case. The number of inputs will always correspond to the number of inputs defined by the circuit description. The input
values are to be applied to the inputs in the order in which the input
operations were defined in the circuit description.
</p>
<p>
The next circuit description, if any, will then follow.
</p><p>
</p><h3>Output</h3>
<p>For each circuit, your program should output one line for each test case given in the input. The line
should contain one `<tt>0</tt>' or `<tt>1</tt>' character for each output defined by the circuit description in the order in
which the outputs were defined.
</p><p>
</p><p>
Your program should output a blank line after each set of test cases.
</p><p>
</p><h3>Example</h3>

<pre><b>Input:</b>

1
00i 11 13 ..
02i 11 13 ..
11&amp; 21 ..
21o ..
13| 23 ..
23o ..
end
4
00
01
10
11

<b>Output:</b>

00
01
01
11
</pre>
<p>
<b>Notes:</b>
</p><ul><li> i, o and ! operations will always have exactly one input.</li><li> &amp; and <tt>|</tt> operations will always have exactly two inputs.</li><li> Even if an operation can feed others, it does not have to.</li><li> No recursive circuits.</li><li> o can also be an input for another gate

</li></ul>
<p>
</p><p>
</p><p>
<b>Hint:</b>
Sample input specifies a circuit consiting of an `AND' and an `OR' operation
in parallel both fed from the same two inputs:
</p><p>
</p><pre>               +---------\
3              |          |OR #----------OUT(2)
               |     +---/
               |     |
2     IN(2)----+     |
               |     |
               +---------\
1                    |    |AND#----------OUT(1)
                     +---/
                     |
0      IN(1)---------+

         0                 1              2</pre>
<p>
In grid terms this is two inputs at 0,0 and 1,0. The first input feeds the <tt>AND</tt> operation at 1,1 and the

<tt>OR</tt> operation at 1,3. The second input operation feeds the second input for the same <tt>AND</tt> and <tt>OR</tt>
operations. The <tt>AND</tt> operation then feeds an output operation at 2,1. The <tt>OR</tt> operation also feeds an output operation, this one at 2,3.
</p><p>
</p>