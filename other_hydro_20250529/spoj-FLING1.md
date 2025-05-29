<p>Fling! is a popular puzzle game created by the well-known developers at CandyCane LLC.</p>
<p style="text-align: center;"><img src="./22438/file/NQNt5o4u.png" alt="" width="320" height="480"></p>
<p>The premise of the game is simple. You are given a certain number of balls on the screen to start. The goal is to fling one into another in order to knock the other off the screen. The puzzle is considered solved if you can do so while leaving only one ball remaining on the screen. Some might read this and think that it might not be too difficult, but the game gets challenging quickly. The problem is that you cannot fling two balls that are adjacent (i.e. next to) each other.</p>
<p>The first ball you choose can fling the 2nd ball if and only if..<br>&nbsp;&nbsp;&nbsp; 1) The two balls exist in same row or same column<br>&nbsp;&nbsp;&nbsp; 2) The two balls are not adjacent<br>&nbsp;&nbsp;&nbsp; 3) There is no other ball in between the two balls</p>
<p>If there exist a 3rd ball after the 2nd ball in the same line of action, the 2nd ball takes the position just before the third ball, pushes the 3rd ball and the 3rd ball gets flinged. (This continues till a ball gets knocked off the screen. Note that 2nd ball and 3rd ball can be adjacent).</p>
<p><br>Given a Fling! puzzle, just print "Yes" if it is a valid puzzle(solvable) or "No" otherwise.<br><br>For better understanding of gameplay you may have a look at this <a href="http://www.youtube.com/watch?v=HfteaRTGyVw">video</a>. (optional)</p>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p><br>The first line of the input consists of an integer t, the number of test cases. For each test case, the first line consists of two integers m and n, the number of rows and columns of the puzzle. Then follows the description of the board. A[i][j] is '.' if the cell is empty or 'B' if the cell has a ball.</p>
<p><strong>Output:</strong></p>
<p>For each test case print "Yes" if the puzzle is valid or "No" otherwise. (case-sensitive).</p>
<p><strong>Input Constraints:</strong></p>
<p>1&lt;=t&lt;=100</p>
<p>1&lt;=m,n&lt;=10</p>
<p>You can assume that the number of balls in the board is approximately equal to ( m x n ) /10<br><br><strong>Sample Input:</strong></p>
<p>4</p>
<p>5 5</p>
<p>.....<strong>&nbsp;</strong></p>
<p>.....</p>
<p>..B..</p>
<p>.....</p>
<p>.B..B</p>
<p>5 4</p>
<p>....</p>
<p>B...</p>
<p>B...</p>
<p>....</p>
<p>B...</p>
<p>3 4</p>
<p>BB..</p>
<p>....</p>
<p>.B..</p>
<p>1 1</p>
<p>B</p>
<p><strong>Sample Output:</strong></p>
<p>Yes</p>
<p>Yes</p>
<p>No<strong>&nbsp;</strong></p>
<p>Yes</p>