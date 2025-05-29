<p>Consider a list of numbers with two operations:</p>
<ul>
<li>insert number — adds the specified number to the end of the list.</li>
<li>delete number — removes the first occurrence of the specified number from the list. If the list&nbsp;does not contain the number specified, no changes are performed.</li>
</ul>
<p>For example: the result of the insertion of a number 4 to the list [1, 2, 1] is the list [1, 2, 1, 4]. If we delete&nbsp;the number 1 from this list, we get the list [2, 1, 4], but if we delete the number 3 from the list [1, 2, 1, 4],&nbsp;the list stays unchanged.</p>
<p>The list is homogeneous if it contains at least two equal numbers and the list is heterogeneous if it&nbsp;contains at least two different numbers. For example: the list [2, 2] is homogeneous, the list [2, 1, 4] is&nbsp;heterogeneous, the list [1, 2, 1, 4] is both, and the empty list is neither homogeneous nor heterogeneous.</p>
<p>Write a program that handles a number of the operations insert and delete on the empty list and&nbsp;determines list’s homogeneity and heterogeneity after each operation.</p>
<h3>Input</h3>
<p>The first line of the input file contains an integer number n — the number of operations to handle&nbsp;(1 ≤ n ≤ 100 000).</p>
<p>Following n lines contain one operation description each. The operation description consists of a word&nbsp;“<tt>insert</tt>” or “<tt>delete</tt>”, followed by an integer number k — the operation argument (−10^9 ≤ k ≤ 10^9 ).</p>
<h3>Output</h3>
<p>For each operation output a line, containing a single word, describing the state of the list after the&nbsp;operation:</p>
<ul>
<li>“<tt>both</tt>” — if the list is both homogeneous and heterogeneous.</li>
<li>“<tt>homo</tt>” — if the list is homogeneous, but not heterogeneous.</li>
<li>“<tt>hetero</tt>” — if the list is heterogeneous, but not homogeneous.</li>
<li>“<tt>neither</tt>” — if the list is neither homogeneous nor heterogeneous.</li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong>
11
insert 1
insert 2
insert 1
insert 4
delete 1
delete 3
delete 2
delete 1
insert 4
delete 4
delete 4

<strong>Output:</strong>
neither
hetero
both
both
hetero
hetero
hetero
neither
homo
neither
neither</pre>