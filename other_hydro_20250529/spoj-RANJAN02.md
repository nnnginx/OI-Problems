<p>Given 3 three pegs: leftmost peg A, middle peg B and rightmost peg C.Find the shortest sequence of moves that transfers a tower of n disks from the left peg A to the right peg C, if direct moves between A and C are disallowed. (Each move must be to or from the middle peg B.)<br><br> Constraints:<br> 1. Initially the left peg A in stacked by n disks in the order of decreasing size.<br> 2. Only one move cand be done at a time and never moving a larger one onto a smaller.<br> 3. Number of moves will always be less than 2^64.<br>4. 1 &lt;= n &lt;= 35</p>
<h3>Input</h3>
<p>Input begins with a integer t, followed by t lines. Each line has the no. of pegs n.</p>
<h3>Output</h3>
<p>For each test case, output the minimum no. of move required to transfer the n disks from peg A to peg C.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>4<br>1<br>2<br>5<br>10<br><br><strong>Output:</strong><br>2<br>8<br>242<br>59048<br></pre>