<p>
An Imp jumps on an infinite chessboard. Moves possible
for the Imp are described by two pairs of integers:
(a,b) and (c,d) - from square (x,y) the Imp
can move to one of the squares: (x+a,y+b), (x-a,y-b),
(x+c,y+d), (x-c,y-d). We want to know for which square
different from (0,0) to which the Imp can jump from (0,0)
(possibly in many moves) the value |x|+|y| is the lowest.
</p>
<h3> Task </h3>
<p>
Write a program which
</p>
<div align="justify">
<ul>
<li> reads from standard input two pairs (a,b) and (c,d) of
integers, different from (0,0), describing moves of the Imp,
</li>
<li> determines a pair of integers (x,y) different from (0,0),
for which the Imp can jump (possibly in many moves) from square (0,0)
to square (x,y) and for which the value |x|+|y| is the lowest.
</li>
<li> writes out to standard output the value |x|+|y|.
</li>
</ul></div>


<h3> Input </h3>
<p>
Ten test cases. Each test consists of four numbers a,b,c,d in one line, separated
by spaces. <br>
-100000 &lt;= a, b, c, d &lt;= 100000
</p>

<h3> Output </h3>
<p>
For every test case your program should write a single line with a number equal the lowest possible value |x|+|y|.
</p>
<h3>Example</h3>
<pre><tt><b>Input:</b>
13 4 17 5
[and 9 test cases more]
<b>Output:</b>
2
[and 9 answers more]
</tt>
</pre>