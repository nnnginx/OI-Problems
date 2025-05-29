<p>
A word is a string of two or more letters while a code is a string of one or more distinct words
in lexicographic order. Thus a string of letters may represent either a word or
a code. An optimum code is a code that contains the maximum number of words.

</p><p>
For a given string of letters there may be one or more optimum codes. The optimum code of top
priority is the optimum code that appears at the top when all optimum codes are arranged in
lexicographic order.

</p><p>
Given a string of letters, you are required to write a program that finds the
following:

</p><p>

</p><ul>
<li>The total number of words, <span class="MATH"><i>m</i></span> in an optimum code,

</li>
<li>The total number of optimum codes, <span class="MATH"><i>n</i></span> represented by the string,
</li>
<li>The optimum code of top priority, the top-code.
</li>
</ul>

<p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001001000000000000000">
Input</a>&nbsp;</font>
</h2>

<p>
Input consists of multiple test cases.

</p><p>
For each test case there is only one line of input. It contains a string of at most
100 letters.

</p><p>
A line consisting of a single letter terminates input.

</p><p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001002000000000000000">
Output</a>&nbsp;</font>
</h2>

<p>
For each test case, present output in two lines.

</p><p>
The first line gives the two integers <span class="MATH"><i>m</i></span> and <span class="MATH"><i>n</i></span> defined above. The next line gives the optimum
code of top priority, the top-code.


</p><p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001003000000000000000">
Sample Input</a>&nbsp;</font>
</h2>

<p>
</p><pre>aaaaaa
words
lexicographic
a
</pre>

<p>

</p><h2><font size="4" color="#ff0000"><a name="SECTION0001004000000000000000">
Sample Output</a>&nbsp;</font>

</h2>

<p>
</p><pre>2 1
aa aaaa
1 1
words
3 2
lexic og raphic
</pre>

<p>
</p><hr><address>Kanpur-Kolkata 2004-2005</address><p>
</p>