<p>
Dyzio is Jasiek's friend and he also likes riddles. Here is a riddle he came up with:
</p>
<div align="justify">
<i>
Jasiek, here is a piece of rope, which has to be cut into smaller pieces.
I will not tell you directly how to do it, but look at this
sequence of zeros (0) and ones (1). A one at the begining means that the rope
has to be cut in half. If the first digit was zero, it would be the only
digit in the sequence and mean you don't have to cut anything - I want
the whole rope. If you have to cut the rope anyway then after the first
1 I wrote what to do with the left piece (according to the same rules as with
the whole rope) and then I wrote what to do with the right piece of rope
(all the time with the same rules of notation). Every time you have to
cut the left piece first, only then can you cut the right one. Now start cutting
and tell me, how many cuts you have to do until you have cut off the shortest piece.
</i>
</div>
<p>
Unfortunately mom hid the scissors from Jasiek, but luckily a computer was at hand
and Jasiek quickly wrote a program simulating the rope cutting. Can you write
such a program?
</p>
<h3> Task </h3>
<p>
Write a program which
</p>
<div align="justify">
<ul>
<li> reads (from standard input) description of the way the rope is cut,
</li>
<li> counts how many cuts have to be made in order to get the first shortest piece.
</li>
<li> writes out the outcome (to standard output)
</li>
</ul></div>
<h3> Input </h3>
<p>
Ten test cases (given one under another, you have to process all!).
Each test case consists of two lines.
In the first line there is a number <i>n (1&lt;=n&lt;=20000)</i>. In the second
line one zero-one word (a sequence of zeros and ones without spaces between them)
of length <i>n</i> - the description of the cutting procedure given by Dyzio.
</p>
<h3> Output </h3>
<p>
For every testcase your program should write (to the standard output) only
one line with one integer equal to the number of
cuts which have to be made in order to get the shortest piece.
</p>
<h3>Example</h3>
<pre><tt><b>Input:</b>
9
110011000
[and 9 test cases more]
</tt>
<tt><b>Output:</b>
4
[and 9 test cases more]
</tt>
</pre>