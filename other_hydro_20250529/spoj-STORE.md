<p>
The floor of a store is a rectangle divided into<i> n*m</i> square
fields. Two fields are adjacent, if they have a common side. A parcel
lays on one of the fields.
Each of the remaining fields is either
empty, or occupied by a case, which is too heavy to be moved by a
store-keeper. The store-keeper has to shift the parcel from the
starting field
<b> P</b> to the
final field <b>K</b>. He can move on the empty
fields, going from the field on which he stands to a chosen adjacent
field. When the store-keeper stays on a field adjacent to the one with
the parcel he may
push the parcel so that if moves to the next field (i.e. the field on
the other side of the
parcel), assuming condition that there are no cases on this field.
</p>

<h3>Task</h3>
<p>
Write a program, which:
</p><ul>
<li>reads from the standard input a store scheme, a starting position of the store-keeper and a final position of the parcel,
</li><li>computes minimal number of the parcel shifts through borders of fields,
  which are necessary to put the parcel in
  the final position or decides that it is
  impossible to put the parcel there,
</li><li>writes the result into the standard output. 
</li></ul>

<h3>Input</h3>

<p>
The number of test cases t is in the first line of input, then t test cases follow separated by an empty line.
In the first line of each test case two positive integers separated by a single space,<i> n,m&lt;=100,</i> are written. These are dimensions of the store. In each
of the following <i> n</i> lines there appears one <i>m</i>-letter word made of letters S, M, P, K, w. A letter on
<i>i</i>-th position in <i>j</i>-th word denotes a type of the field with coordinates
(<i>i,j</i>) and its meaning is following:&nbsp;</p>
<ul>
<li>S - case,
</li><li>M - starting position of the store-keeper,
</li><li>P - starting position of the parcel,
</li><li>K - final position of the parcel,
</li><li>w - empty field.&nbsp;
</li></ul>
<p>Each letter M, P and K appears in the test case exactly once.</p>

<h3>Output</h3>
<p>
Your program should write to the standard output for each test case:&nbsp;
</p><ul>
<li>exactly one word NO if the parcel cannot be put on the target
  field,
</li><li>exactly one integer, equal to the minimal number of the parcel
shifts through borders of the fields, necessary to put a parcel on a
final position, if it is possible to put the parcel there.
</li></ul>

<h3>Example</h3>
<pre><b>Sample input:</b>
1
10 12
SSSSSSSSSSSS
SwwwwwwwSSSS
SwSSSSwwSSSS
SwSSSSwwSKSS
SwSSSSwwSwSS
SwwwwwPwwwww
SSSSSSSwSwSw
SSSSSSMwSwww
SSSSSSSSSSSS
SSSSSSSSSSSS

<b>Sample output</b>
7
</pre>