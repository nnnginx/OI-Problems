<div align="justify">
<p>
Jack has got a new game of Super Mario recently. There are <b>n</b> castles in the game, and Princess Peach has been kidnapped by the King Koopa and enjailed in castle n - 1 (0-based). The King Koopa has Son Koopas, and the Son Koopas has Grandson Koopas, and the Grandson Koopas has Great-Grandson Koopas... The whole Koopa family is taking possession of these n castles, and there is exactly one Koopa in each castle and the King Koopa is in castle n - 1. Super Mario's task is to conquer these castles and save Princess Peach. </p>
<p>
Each time, Super Mario can freely choose an unconquered castle and go in to fight with the Koopa. Super Mario has time <b>T[i]</b> to conquer castle <b>i</b> and beat the Koopa in it. If Super Mario fails to conquer the castle or fails to do that within the time limit, the game is over. Otherwise, the defeated Koopa will go to seek the Father Koopa for help. If any Koopa has two or more Son Koopas beaten by Super Mario, he will get angry. Super Mario has to go to the castle of the angry Koopa and beat him immediately; otherwise the Princess Peach will be killed. If castle n - 1 is conquered and King Koopa is defeated, the game will also end, but with triumph and Princess Peach saved.</p>
<p>
Jack loves this game a lot, but he has to prepare for the upcoming ACM/ICPC. So he guarantees to himself that he only plays the game once a month. However, Jack really loves playing game and hates programming, he wants to maximize the time he can spend on the game without breaking his promise.
</p>
<br>
<b>Input Format:</b><br>
The input consists of multiple test cases.<br>
Each test case starts with a number <b>N</b> (0 &lt; N &lt;= 100,000) in a single line, the number of castles and Koopas. There are two lines following and each contains N numbers. <br>
The first line is N numbers, <b>T[i]</b> (0 &lt; <b>T[i]</b> &lt;= 100) for Super Mario to conquer castle i. <br>
The second line is N numbers of <b>P[i]</b> (-1 &lt;= Pi &lt; N), the castle (0-based) in which the Parent of each Koopa resides. <br>
-1 means that there is no parent for him, and the last number will always be -1, since King Koopa has no Parent Koopa.

The input ends with 0(zero), which should not be processed.<br>
<br>
<b>Output Format:</b><br>
Output the maximal time Jack can play in a single line for each test case.<br>
<br>
<b>Sample Input:</b><br>
<pre>5
1 2 3 4 5
4 4 4 4 -1
5
2 2 2 2 2
1 2 3 4 -1
9
1 1 1 1 1 1 1 1 1
6 6 6 7 7 7 8 8 -1
0
</pre>

<b>Sample Output:</b><br>
<pre>12
10
8    
</pre>
</div>