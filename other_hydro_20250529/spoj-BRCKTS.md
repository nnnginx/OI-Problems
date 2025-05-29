<p>
We will call a <b>bracket word</b> any word constructed out of two sorts
of characters: the opening bracket "(" and the closing bracket ")". Among
these words we will distinguish <b>correct bracket expressions</b>. These are
such bracket words in which the brackets can be matched into pairs such that
</p><ul>
<li>every pair consists of an opening bracket and a closing bracket
appearing further in the bracket word</li>
<li>for every pair the part of the word between the brackets of this pair
has equal number of opening and closing brackets
</li>
</ul>

On a bracket word one can do the following operations:
<ul>
<li><b>replacement</b> -- changes the i-th bracket into the opposite one</li>
<li><b>check</b> -- if the word is a correct bracket expression</li>
</ul>
<p></p>
<h3>Task</h3>
<p>
Write a program which
</p>
<div align="justify">
<ul>
<li> reads (from standard input) the bracket word and the sequence of
operations performed,
</li>
<li> for every check operation determines if the current bracket word is
a correct bracket expression,
</li>
<li> writes out the outcome (to standard output).
</li>
</ul></div>

<h3>Input</h3>
<p>
 Ten test cases (given one under another, you have to process all!).
 Each of the test cases is a series of lines.
 The first line of a test consists of a single number <i>n (1&lt;=n&lt;=30000)</i> denoting
 the length of the bracket word.
 The second line consists of <i>n</i> brackets, not separated by any spaces.
 The third line consists of a single number <i>m</i> -- the number of operations.
 Each of the following <i>m</i> lines carries a number <i>k</i> denoting the operation
 performed. <i>k=0</i> denotes the check operation, <i>k&gt;0</i> denotes replacement of
 <i>k</i>-th bracket by the opposite.
</p>
<h3>Output</h3>
<p>
For every test case your program should print a line:<br>
Test i:<br>
where i is replaced by the number of the test
and in the following lines, for every check operation in the i-th test
your program should print a line with the word
YES,
if the current bracket word is a correct bracket expression, and a line
with a word
NO otherwise.
(There should be as many lines as check operations in the test.)
</p>
<h3>Example</h3>
<pre><tt><b>Input:</b>
4
()((
4
4
0
2
0
[and 9 test cases more]
<b>Output:</b>
Test 1:
YES
NO
[and 9 test cases more]
</tt>
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>