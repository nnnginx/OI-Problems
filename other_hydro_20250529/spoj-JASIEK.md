<p>
Jasiek is only 6 years old, but he already has many skills.
He likes drawing and asking riddles very much. This morning he got
a sheet of grid paper and a pencil from his mother and he
started drawing. All his drawings have some common properties:
</p>
<div align="justify">
<ul>
<li>Jasiek colors full grid squares;</li>
<li>if some coloured grid squares touch each other, it means they have
a common edge or a corner;</li>
<li>all grid squares are connected, which means between every two coloured grid squares
there is a sequence of coloured grid squares, which have a common edge;</li>
<li>there are no white holes, that is from every white grid box it is possible to draw a line to the boundary of the sheet which never touches any coloured grid square.</li>
</ul>
</div>
<p>At noon mom phoned and asked what Jasiek's today's picture was. The boy didn't answer directly, but described the picture by a sequence of moves needed to walk around
the centres of the coloured squares on its boundary, ie. those squares which
have at least one common corner with a white square. Jasiek set the starting square
and then gave the sequence of moves necessary to walk along the boundary squares anti-clockwise. Mom was very surprised by the complexity of the picture and especcialy
by the number of coloured squares. Given Jasiek's description, can you quickly count how many coloured squares there are in the picture?
</p>
<h3>Task</h3>
<p>
Write a program which
</p>
<div align="justify">
<ul>
<li> reads (from standard input) Jasiek's description of the picture,
</li>
<li> counts the number of coloured squares,
</li>
<li> writes out the outcome (to standard output).
</li>
</ul></div>
<h3>Input</h3>
<p>
Ten test cases (given one under another, you have to process all!).
Each of the test cases is a series of lines. Each line consists of only one character.
The letter <i>P</i> means the beginning of the description.
The letter <i>K</i> means the end of the desription (and the test case). All other lines (if any) contain one of the letters N, W, S or E (N meaning North, W - West, S - South and E - East). Every line of the description
corresponds to the relative position of the centre of some square on the boundary of the picture. The first and the last
line correspond to the same square. A letter in a line other than the first or the last tells you which way you have to go in order to get to the next boundary square when going around the picture anti-clockwise. Jasiek's description finishes after going around the picture once. The length of the description doesn't exceed 20000 letters.
</p>
<h3> Output </h3>
<p>
For every testcase your program should write (to the standard output) only
one line with one integer, equal to the number of coloured squares in Jasiek's picture.
</p>
<h3>Example</h3>
<img src="/content/kfas:JAS.png" alt="Example illustration">
<p>
</p><pre><tt><b>Input:</b>
P
S
S
S
E
N
E
E
S
E
E
N
N
N
N
S
S
S
W
W
N
N
W
W
W
N
S
K
[and 9 test cases more]
</tt>
<tt><b>Output:</b>
23
[and 9 test cases more]
</tt>
</pre>