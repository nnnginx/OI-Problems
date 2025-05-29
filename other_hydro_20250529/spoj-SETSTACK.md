<p>
<img src="./24311/file/b2Gm0W7H.png">
</p>
<p>
Background from Wikipedia:
<q>Set theory is a branch of mathematics created principally by the
German mathematician Georg Cantor at the end of the 19th
century. Initially controversial, set theory has come to play the role
of a foundational theory in modern mathematics, in the sense of a
theory invoked to justify assumptions made in mathematics concerning
the existence of mathematical objects (such as numbers or functions)
and their properties. Formal versions of set theory also have a
foundational role to play as specifying a theoretical ideal of
mathematical rigor in proofs.</q>
</p>
<p>
Given this importance of sets, being the basis of mathematics, a set
of eccentric theorist set off to construct a supercomputer operating on
sets instead of numbers. The initial SetStack Alpha is under
construction, and they need you to simulate it in order to verify the
operation of the prototype.
</p>
<p>
The computer operates on a single stack of sets, which is initially
empty. After each operation, the cardinality of the topmost set on the
stack is output. The cardinality of a set <em>S</em> is denoted
|<em>S</em>| and is the number of elements in <em>S</em>.  The
instruction set of the SetStack Alpha is <tt>PUSH</tt>, <tt>DUP</tt>,

<tt>UNION</tt>, <tt>INTERSECT</tt>, and <tt>ADD</tt>}.

</p><ul>
<li> <tt>PUSH</tt> will push the empty set {} on the stack.
</li><li> <tt>DUP</tt> will duplicate the topmost set (pop the stack, and then push that set on the stack twice).
</li><li> <tt>UNION</tt> will pop the stack twice and then push the union of the two sets on the stack.

</li><li> <tt>INTERSECT</tt> will pop the stack twice and then push the intersection of the two sets on the stack.
</li><li> <tt>ADD</tt> will pop the stack twice, add the first set to the second one, and then push the resulting set on the stack.
</li></ul>
<p></p>
<p>
For illustration purposes, assume that the topmost element of the stack is 
</p><p>
<em>A</em> = { {}, {{}} },
</p>
<p>

and that the next one is
</p>
<p>
<em>B</em> = { {}, {{{}}} }.
</p>
<p>
For these sets, we have |<em>A</em>| = 2 and |<em>B</em>| = 2. Then:
</p><ul>
<li> <tt>UNION</tt> would result in the set { {}, {{}}, {{{}}} }.  The
output is 3.
</li><li> <tt>INTERSECT</tt> would result in the set { {} }.  The output is 1.

</li><li> <tt>ADD</tt> would result in the set { {}, {{{}}}, {{},{{}}} }.
The output is 3.
</li></ul>
<p></p>
<h3>Input</h3>
<p>
An integer 0 ¡Ü <em>T</em> ¡Ü 5 on the first line gives the
cardinality of the set of test cases. The first line of each test case
contains the number of operations 0 ¡Ü <em>N</em> ¡Ü 2000. Then
follow <em>N</em> lines each containing one of the five commands. It
is guaranteed that the SetStack computer can execute all the commands
in the sequence without ever popping an empty stack.
</p>

<h3>Output</h3>
<p>
For each operation specified in the input, there will be one line of
output consisting of a single integer. This integer is the cardinality
of the topmost element of the stack after the corresponding command
has executed. After each test case there will be a line with
<tt>***</tt> (three asterisks).
</p>
<h3>Example</h3>

<pre><b>Input:</b>
2
9
PUSH
DUP
ADD
PUSH
ADD
DUP
ADD
DUP
UNION
5
PUSH
PUSH
ADD
PUSH
INTERSECT

<b>Output:</b>
0
0
1
0
1
1
2
2
2
***
0
0
1
0
0
***
</pre>