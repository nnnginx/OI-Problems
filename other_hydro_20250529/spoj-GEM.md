<p>You are given a board with 8*8 squares. In each square, there can be either a colored gem or no gem at all. Gems with different colors are represented by different integers. It is guaranteed that there are no more than two consecutive gems with the same color either in a row or in a column.</p>
<pre>........
........
........
........
........
..43366.
..121556
44212335
</pre>
<p>For two neighboring (up, down, left or right, we don't consider diagonal neighbors) squares, you can exchange the gems.</p>
<pre>........
........
........
........
........
..43366.
..111556
44222335
</pre>
<p>You can also exchange a gem with a space. After that, if there are more than two consecutive gems with the same color in a row or in a column after exchange, these gems will be taken away simultaneously. Note that a gem could be counted both in its row and in its column; refer to the sample test cases for details.</p>
<pre>........
........
........
........
........
..43366.
.....556
44...335
</pre>
<p>If there is no gem under a gem, the gem will fall to the square below.</p>
<pre>........
........
........
........
........
.....66.
.....556
44433335
</pre>
<p>After all the squares falling down to the floor or another gem square, repeat the procedure until there's no gem can be taken away: if there are more than two gems with the same color in a row or in a column, these gems will be taken away simultaneously. Then some gems will fall to the squares below, if there are no gems under those gems.</p>
<pre>........
........
........
........
........
.....66.
.....556
.......5

........
........
........
........
........
........
.....666
.....555

........
........
........
........
........
........
........
........
</pre>
<p>Given a board with 8*8 squares. This board is stable and you can't take away any gems in the original board. Your task is to determine whether all gems can be taken away by a single exchange or not.</p>
<h3>Input</h3>
<p>The input consists of several test cases. Each test case will be eight lines, and each line contains eight characters. If in a square there is no gem, ��.�� is used to identify it, otherwise an integer <em>k</em> is used to identify the gem's color, 1&lt;= <em>k</em> &lt;=9.</p>
<p>There is a blank line between two consecutive test cases.</p>
<p>End of input is indicated by a line consisting of 0.</p>
<h3>Output</h3>
<p>For each test case, output a single line. If all gems can be taken away by a single exchange, output <strong>Yes</strong>; otherwise output <strong>No</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
........
........
........
........
........
..43366.
..121556
44212335

........
........
........
.2......
.2.22...
.1.11...
.2.22...
.2.22...

12121212
21212121
12121212
21212121
12121212
21212121
12121212
21212121

........
........
........
........
........
...96...
...96...
.996966.

0

<strong>Output:</strong>
Yes
Yes
No
Yes
</pre>