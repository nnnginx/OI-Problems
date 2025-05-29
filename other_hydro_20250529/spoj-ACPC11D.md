<p>You and your friends like to play chess and backgammon &nbsp;every day. &nbsp;But now you are bored of these games, and you would like to play a new game. &nbsp;So you decided to make your own game, which will be played using a backgammon&nbsp; die (singular of dice) on a board similar to the chess board, and it will be a single player game.</p>
<p><a title="ImageShack - Image And Video Hosting" href="http://imageshack.us/photo/my-images/266/imau.png/" target="_blank"><img src="./21118/file/bLdRJtNC.png" border="0" alt=""></a></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">&lt;a target='_blank' title='ImageShack - Image And Video Hosting' href='http://imageshack.us/photo/my-images/266/imau.png/'&gt;&lt;img src='http://img266.imageshack.us/img266/6522/imau.png' border='0'/&gt;&lt;/a&gt;</div>
<p>The game is played on a board of N rows and M columns. &nbsp;Each cell is either empty or contains a number from 0 to 9, and &nbsp;there &nbsp;is a single die (a die with six faces containing the numbers from 1 to 6) placed in one of the empty cells (the borders of the bottom face is aligned to the</p>
<p>axes of the board), &nbsp;and your goal is to move it to a target &nbsp;empty cell.</p>
<p>&nbsp;</p>
<p>The initial orientation of the die is defined by a string S which is a permutation of the digits from 1 to 6. Each digit represents &nbsp;the number written &nbsp;on a face of the die according to this order: right, left, back, front, top, bottom. &nbsp;Moving the die is defined by the following rules:</p>
<p>&nbsp;</p>
<p>1. You can move the die from a cell to one of its four adjacent cells by flipping it on the corresponding face. For example, if the current orientation &nbsp;of the die is 136425 and you will move it to the cell on its right,&nbsp; you should flip the die on its right face and it will become the bottom &nbsp;face in the right cell, so the orientation of the die will be 256431. (This is the example in the figure).</p>
<p>2. Your score is initially &nbsp;zero. &nbsp;By moving the&nbsp; die to another &nbsp;cell, if the&nbsp; number &nbsp;on the bottom &nbsp;face is the same as the number in the cell you just moved to, your score will be increased by the sum of these two numbers, &nbsp;otherwise your score will be decreased by the sum of these two numbers. &nbsp;Entering &nbsp;the target &nbsp;cell will not affect your score.</p>
<p>3. You can not leave the board.</p>
<p>4. Once you leave the starting &nbsp;cell, you can not enter it again.</p>
<p>5. Once you enter the target &nbsp;cell, you can not leave it.</p>
<p>6. You can not enter an empty cell, except the target &nbsp;one.</p>
<p>&nbsp;</p>
<p>Given the board configuration, the starting &nbsp;cell, the target cell and the die��s initial orientation, your task is to move the die from the starting &nbsp;cell to the target &nbsp;cell according the rules above, such that &nbsp;you end up with the maximum &nbsp;possible score. &nbsp;Can you write a program &nbsp;to help you?</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>Your program &nbsp;will be tested &nbsp;on one or more test cases. The first line of the input &nbsp;will be a single integer T , the number of test cases (1 �� T �� 200). After that &nbsp;follow the specifications&nbsp;of T test &nbsp;cases.</p>
<p>Each &nbsp;test &nbsp;case is specified in N + 2 lines. &nbsp;The &nbsp;first line contains &nbsp;two &nbsp;integers &nbsp;N &nbsp;and &nbsp;M&nbsp;(1 �� N, M &nbsp;�� 10) representing &nbsp;the &nbsp;number &nbsp;of rows and &nbsp;number &nbsp;of columns of the &nbsp;board,&nbsp;respectively. &nbsp;The second line contains the string S representing &nbsp;the initial orientation &nbsp;of the die in the starting &nbsp;cell as described above. &nbsp;Each line of the remaining &nbsp;N&nbsp; lines contains &nbsp;M characters, &nbsp;the j-th character &nbsp;in the i-th line represents &nbsp;the value of the j-th cell in the i-th row of the board. &nbsp;Each character &nbsp;will be one of the following values:</p>
<p>1. '.' means an empty cell.</p>
<p>2. 'S' means the starting &nbsp;cell (which will appear &nbsp;exactly once in the board).</p>
<p>3. 'T' means the target &nbsp;cell (which will appear &nbsp;exactly once in the board).</p>
<p>4. A digit from '0' to '9' means the value written &nbsp;in this cell.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test &nbsp;case, output, on a single line, one of these values:</p>
<p>1. "Impossible" if you can not reach the target &nbsp;cell from the starting &nbsp;cell.</p>
<p>2. "Infinity" if there &nbsp;is no limit &nbsp;for your final score, and &nbsp;you can increase it &nbsp;with &nbsp;no&nbsp;limit.</p>
<p>3. Otherwise, &nbsp;output the maximum score which you can get.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
4 4
123456
S789
0987
789.
09.T
3 6
153462
S16521
.46324
.....T
4 4
623451
S6T.
....
....
....


<strong>Output:</strong>
Impossible
Infinity
12
</pre>