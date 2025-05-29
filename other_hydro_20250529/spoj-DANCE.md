<p>
The Gordian Dance is a traditional Bytelandian dance performed by two pairs
of dancers. At the beginning the dancers are standing in the corners of the square <i>ABCD</i>,
forming two pairs: <i>A-B</i> and <i>C-D</i>. Every pair is holding an outstretched string. So in the starting position both strings are stretched horizontally and
parallel.
</p>
<img src="/content/kfas:DANCE1.png" alt="The starting position of dancers.">
<p>The dance consists of a series of moves. There are two kinds of moves:
</p><div align="justify">
<ul>
<li>(<i>S</i>) The dancers standing at points <i>B</i> and <i>C</i>
swap positions (without releasing their strings) in such a way that
the dancer standing at <i>B</i> raises the hand in which he is holding the string and, when going to point <i>C</i>, lets the dancer going from <i>C</i> to <i>B</i>
pass in front of him, under his arm.
</li>
<li>(<i>R</i>) All dancers make a turn by 90 degrees clockwise without releasing their strings.
This means that the dancer from <i>A</i> goes to <i>B</i>,
the dancer from <i>B</i> goes to <i>C</i>,
the dancer from <i>C</i> goes to <i>D</i>,
and the dancer from <i>D</i> goes to <i>A</i>.
</li>
</ul>
</div>
<p>
During the dance the strings tangle with each other, but in the end
they should be untangled and stretched horizontally and parallel.
The dancers do not have to occupy the same spots as in the begining.
The dance requires a lot of experience, because the strings can be extremely tangled during the dance. The sequence of moves after which they are no longer tangled and are stretched horizontally and parallel can be difficult to guess.
</p>
<p>Your program should help beginner dancers end a dance. You are to determine the
minimal number of mover required to end the dance given a sequence of
moves already performed.
</p>
<h3>Illustration</h3>
<p>For example after the sequence <i>SS</i> we get the following configuration.
</p>
<img src="/content/kfas:DANCE2.png" alt="The configuration after SS">
<p>
The shortest sequence of moves required to end the dance is of length 5: <i>RSRSS</i>.
</p>
<h3> Task </h3>
<p>
Write a program which
</p>
<div align="justify">
<ul>
<li>reads from standard input the moves made in a dance,</li>
<li> finds the minimal number of moves required to untangle the strings and
stretch them horizontally and parallel (the dancers don't have to be in their starting spots).
</li>
<li> writes the outcome to standard output.
</li>
</ul>
</div>
<h3> Input </h3>
<p>
Ten test cases (given one under another, you have to process all!). The first line of each test case consists of one integer <i>n</i>
equal to the nmber of moves already made, <i>0&lt;=n&lt;=1000000</i>.
The second line of each test case consists of one word of length <i>n</i>,
made up of letters <i>S</i> and/or <i>R</i>.
</p>
<h3>Output</h3>
<p>
For every testcase your program should write to standard output only
one line with one integer number: the minimal number of
moves required to untangle the strings and stretch them horizontally and parallel.
</p>
<h3>Example</h3>
<pre><tt><b>Input:</b>
2
SS
[and 9 test cases more]
</tt>
<tt><b>Output:</b>
5
[and 9 test cases more]
</tt>
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>