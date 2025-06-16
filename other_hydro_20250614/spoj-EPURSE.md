Jack plays this ball game for the first time in his club. Jack has a ball, which bounces with a width of <b>W</b>. Coins are arranged on a straight line at regular intervals. If the ball strikes the i-th coin, Jack gains <b>money</b>[i] (which could possibly be negative). Jack can take atmost <b>B</b> turns, to throw the ball. At each turn, jack can either throw the ball from left to right, or right to left, and choose which ball to start the knock out. If he chooses to knock out from ball i to the right, he will knock out i, i+W, i+2W, ...; Similarly if he chooses to knock out from right to left, starting from ball i he will knock out, i, i-W, i-2W, ...; Please note that once a ball is knocked out, it is removed and it's place contains a void. i.e., you cant gain <b>money[i]</b> for the same <b>i</b> twice.<br>
Jack wants to maximise his money gained, by carefully choosing his turns. If there is more than one way to gain the same money, jack wishes to minimise the number of times he throws.
<p></p>
<h3>Input Format</h3>
<p>
The input file consists of multiple testcases. <br>
The first line of each testcase contains three integers, <b>W B N</b> (1 &lt;= N &lt;= 100; W,B &gt; 0) <br>
The second line of each testcase contains N integers, denoting <b>money[i]</b>. (| money[i] | &lt;= 10<sup>6</sup>)<br>
Input terminates with a line containing three zeros which must not be processed.

</p><h3>Output Format</h3>

<p>For each testcase print one line denoting the maximal money gained and the number of turns taken. Please see the sample output and stick to the output format.<br>
<i>"Case#id: Jack wins $X out of Y throws."</i><br>
<b>NOTE:</b> You must spell the same way the sample output says. Extra spaces and case insensitivity can cause wrong answer responses.<br>
<br>
<b>Testdata:</b><br>
100 testcases, Timelimit: 10s<br>
<br>
<b>Sample Input:</b><br>
</p><pre>2 3 10
-1 3 2 5 1 -2 0 5 1 -3
2 3 14
-1 3 2 5 -5 -5 1 -2 0 5 -5 -5 1 -3
3 3 5
-1 -2 -3 -4 -5
1 2 6
-1 -1 10 10 -1 -1
0 0 0
</pre>

<b>Sample Output:</b><br>
<pre>Case#1: Jack wins $15 out of 2 throws.
Case#2: Jack wins $10 out of 3 throws.
Case#3: Jack wins $0 out of 0 throws.
Case#4: Jack wins $18 out of 1 throws.
</pre>
<p><b>Output Explanation:</b><br>
We present one of the optimal solutions. We number balls from 1 to N.<br>
TestCase#1: [Jack takes only two throws, though he can take three]<br>
Throw#1: From ball#3 towards right, 2 + 1 + 0 + 1 = 4<br>
Throw#2: From ball#8 towards left, 5 + -2 + 5 + 3 = 11<br>
TestCase#2:<br>
Throw #1: From ball#3 towards left, 2 + -1 = 1<br>
Throw #2: From ball#4 towards left, 5 + 3 = 8<br>
Throw #3: From ball#13 towards right, 1 = 1<br>
TestCase#3:<br>
All numbers are negative. Jack takes no throws.<br>
</p>