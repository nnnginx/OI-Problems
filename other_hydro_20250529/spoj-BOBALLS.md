<p>Consider a grid having NxM squares. The top left square is (0,0) and the bottom right is (N-1,M-1). Each square in the grid is either occupied by a platform or has a number written on it. Two balls are released from the top of the grid (from locations (0,Y1) and (0,Y2), 0 &lt;= Y1,Y2 &lt; M). Each ball falls down vertically, unless either it falls down the bottom row, or encounters a platform beneath. When the ball encounters a platform beneath, it rolls either to the left or to the right, each with an equal probability. The score obtained by a ball is the sum of the numbers on the squares that it passes (including the starting square). However, if both the balls pass over the same square, points corresponding to that square are obtained only once, and not twice. Your goal is to choose Y1 and Y2 such that the expected score obtained by the two balls is maximized. For example, consider the grid below : (P reprsents a platform)</p>
<pre>N = 6, M = 6
112214
211243
30PPP2
423378
1P9753
220102
</pre>
<p>Here, dropping a ball from position (0,3) could result in one of the following three scores :</p>
<pre>1) 2 + 2 + 1 + 1 + 0 + 2 + 4 + 1 + 2 = 15 
2) 2 + 2 + 1 + 1 + 0 + 2 + 3 + 9 + 0 = 20
3) 2 + 2 + 4 + 3 + 2 + 8 + 3 + 2 = 26
</pre>
<p>The expected score is (considering only 1 ball) :</p>
<pre>1/2*(1/2*(15) + 1/2*(20)) + 1/2*(26)</pre>


<h3>Input</h3>
<p>The first line contains the number of test cases.</p>
<p>The first line for each test case consists of N and M.</p>
<p>Lines 2..N+1 for each test case consist of M characters each. Each character is either a digit from 0 to 9, or the letter 'P'.</p>

<h3>Output</h3>
<p>The maximum expected score accurate upto 4 decimal places. </p>

<h3>Example</h3>

<pre><b>Input:</b>
4
5 5
53214
53214
53214
54214
53214
5 5
00000
0P0P0
00000
01P20
00000
5 5
09090
0P0P0
00000
01P20
00000
6 6
112214
211243
30PPP2
423378
1P9753
220102


<b>Output:</b>
45.0000
2.2500
19.3125
35.5000

</pre>

<h3>Constraints</h3>
<p>Dataset 1: 1 &lt;= number of test cases &lt;= 100</p>
<p>
3 &lt;= N,M &lt;= 100</p>
<p>All possible paths from the top will eventually lead to the ball falling from the bottom. There will be no "rebounds" possible. If there is a 'P' on square (x,y), there will not be a 'P' on squares (x-1,y-1) or (x-1,y+1) or (x+1,y-1) or (x+1,y+1). Also, platforms will not occur on the boundaries of the grid. Thus, the X coodinate of a platform will never be 0 or N-1, and the Y coordinate will never be 0 or M-1. The test case was generated to guarantee that any answer with absolute error in 1e-9 will got accepted.
Time limit: 7s</p>