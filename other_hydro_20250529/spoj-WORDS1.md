<p align="justify">
Some of the secret doors contain a&nbsp;very interesting word puzzle. The team of
archaeologists has to solve it to open  that doors. Because there is no
other way to open the doors, the puzzle is very important for us.

</p><p align="justify">
There is a&nbsp;large number of magnetic plates on every door. Every plate has one
word written on it. The plates must be arranged into a sequence in such a way that
every word begins with the same letter as the previous
word ends. For example, the word ``ac<u>m</u>'' can be followed by the word
``<u>m</u>otorola''. Your
task is to write a computer program that will read the list of words and
determine whether it is possible to arrange all of the plates in
a&nbsp;sequence (according to the given rule) and consequently to open the door.


</p><h3>Input</h3>

<p align="justify">The input consists of <var>T</var> test cases. The number of them (<var>T</var>, equal to about 500) is given on
the first line of the input file.
Each test case begins with a line containing a&nbsp;single integer number <var>N</var> that indicates the number of plates
(<var>1 &lt;= N &lt;= 100000</var>). Then exactly <var>N</var>lines follow,
each containing a&nbsp;single word. Each word contains at least two
and at most 1000 lowercase characters, that means only letters '<code>a</code>'
through '<code>z</code>' will appear in the word. The same word may appear several
times in the list.


</p><h3>Output</h3>

<p align="justify">Your program has to determine whether it is possible to arrange all the plates in
a&nbsp;sequence such that the first letter of each word is equal to the last
letter of the previous word. All the plates from the list must be used, each
exactly once. The words mentioned several times must be
used that number of times.

</p><p align="justify">
If there exists such an ordering of plates, your program should print 
the&nbsp;sentence "<code>Ordering is possible.</code>". Otherwise, output
the&nbsp;sentence "<code>The door cannot be opened.</code>".


</p><h3>Example</h3>
<pre><b>Sample input:</b>
3
2
acm
ibm
3
acm
malform
mouse
2
ok
ok

<b>Sample output:</b>
The door cannot be opened.
Ordering is possible.
The door cannot be opened.</pre>

<p><b>Warning: large Input/Output data, be careful with certain languages</b></p>