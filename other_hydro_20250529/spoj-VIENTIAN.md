<p>The Tower of Hanoi is a mathematical game or puzzle. It consists of three rods, and a number of disks of different sizes which can slide onto any rod. The puzzle starts with the disks neatly stacked in order of size on one rod, the smallest at the top, thus making a conical shape.
The objective of the puzzle is to move the entire stack to another rod, obeying the following rules:
</p><ul>
<li>Only one disk may be moved at a time.</li>
<li>Each move consists of taking the upper disk from one of the rods and sliding it onto another rod, on top of the other disks that may already be present on that rod.</li>
<li>No disk may be placed on top of a smaller disk.</li>
</ul><p></p>
<p>It is known that the puzzle can be solved in <b>2<sup>n</sup>-1</b> steps for n disks.</p>
<p>Now consider the puzzle called The Tower of Vientiane. The rules are almost the same as for The Tower of Hanoi. But additionally there are limitations on the allowed moves. Let the initial rod be numbered 1, the target rod - 3, and the auxiliary rod - 2. The matrix of allowed moves is given. For example is can be allowed to move disks from rod 1 to rod 2 only, from rod 2 to rod 3 and from rod 3 to rod 1. You are to find out the minimal number of moves in which the puzzle can be solved given some limitations on the allowed moves.</p>

<h3>Input</h3>
<p>The first line of the input contains number <b>t</b> ¨C the amount of tests. Then <b>t</b> test descriptions follow. The test starts with a <b>3x3</b> matrix, consisting of <b>1s</b> and <b>0s</b>. The <b>1</b> in <b>i-th</b> row and <b>j-th</b> column of the matrix means that the move from rod <b>i</b> to rod <b>j</b> is allowed, otherwise it is not allowed. The next line of each test contains the number <b>n</b> - the amount of disks for the corresponding testcase.

</p><h3>Constraints</h3>
<p>1 &lt;= <b>t</b> &lt;= 10000<br>
2 &lt;= <b>n</b> &lt;= 39</p>

<h3>Output</h3>
<p>For each test print the minimal number of moves in which the puzzle can be solved or "Epic Fail..." if it's impossible to solve the puzzle under such limitations.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
011
101
110
5
010
101
010
5
010
001
010
5


<b>Output:</b>
31
242
Epic Fail...

</pre>