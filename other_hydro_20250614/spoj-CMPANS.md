<p>In a place in Southwestern Europe, the name of which I do not wish to recall, not long ago there were <em>n</em> cities connected by unidirectional roads, with possibly more than one road connecting a city to another one, or even to itself. As a homework assignment for your geography class, you need to calculate the number of paths of length exactly two that were between each pair of cities. However, you��ve been too busy celebrating the Spanish victory in the World Cup, so now you are copying the answers from your friend. You would like to make sure his answers are correct before handing in your homework.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The input consists of several test cases, separated by single blank lines. Each test case begins with a line containing the integer <em>n</em> (1 �� <em>n</em> �� 700). The following <em>n</em> lines contain <em>n</em> elements each, with element <em>j</em> of line <em>i</em> being the number of roads from city <em>i</em> to city <em>j</em> (a number between 0 and 10, inclusive). After that, there will be <em>n</em> lines. Each will contain <em>n</em> elements, with element <em>j</em> of line <em>i</em> being the answer from your friend for the number of length-2 paths from city <em>i</em> to city <em>j</em>; it will be an integer between 0 and 100&nbsp;000 inclusive.</p>
<p>The test cases will finish with a line containing only the number zero (also preceded by a blank line).</p>
<p><strong>Note:</strong> Large input file; use fast I/O routines (e.g. scanf in C++ or BufferedReader in Java).</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>For each case, your program should output a line. The content of this line should be <tt>YES</tt> if your classmate��s solution to the assignment is right, and <tt>NO</tt> otherwise.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">3
2 0 1
1 0 3
1 1 0
5 1 2
5 3 1
3 0 4

3
2 0 1
1 0 3
1 1 0
5 1 2
5 3 2
3 0 4

0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">YES
NO
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Abel Molina Prieto</em></blockquote>