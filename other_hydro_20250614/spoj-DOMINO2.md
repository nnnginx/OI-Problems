<p>You have an <b>n</b>x<b>m</b> rectangle, some cells have some obstacles in. A domino piece is a 1x2 or 2x1 rectangle. You're going to place some domino pieces in this rectangle so that there's no empty cell is covered more than once and no cell with obstacles is covered. For some unknown reason, you have to ensure there's at least one piece covering some cell in row i and some cell in row i+1 at the same time for all i in 1..<b>n</b>-1. Similarly there's at least one piece covering some cell in column i and column i+1 for all i in 1..<b>m</b>-1. Your task is to count the number of different valid domino covering.</p>

<h3>Input</h3>
<p>The first line of the input contains two integer numbers <b>n</b>, <b>m</b> (1¡Ü<b>n</b>,<b>m</b>¡Ü15).</p>
<p>The following <b>n</b> lines describe the rectangle. Each line contains <b>m</b> characters. The j-th character of line i+1 may be either a '<tt>x</tt>'(ASCII code 120), representing obstacles in cell (i, j), or a '<tt>.</tt>'(ASCII code 46), representing an empty cell. </p>

<h3>Output</h3>
<p>One number, representing the number of different valid domino placing.</p>
<p>Since the number could be quite large, output the answer modulo 19901013.</p>

<h3>Example</h3>

<pre><b>Input:</b>
3 3
...
...
...

<b>Output:</b>
2
</pre>

<h3>Note</h3>
<p>The 2 different placings are</p>
<pre>   112     411
   4.2     4.2
   433     332
</pre>