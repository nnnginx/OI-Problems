<p>The television at the boy's home contains the channels from 1 to n inclusive. The father wanted to avoid his son to watch some channels in the Television. You are given k unique channels that are banned by the father. <br>For example assume that the TV contains 25 channels and the father bans the channels 15, 17 and 18 and you are currently at channel 16. If you press the 'down' button in the remote,&nbsp; you will move to channel 14 and if you press the 'up' button in the remote, you will move to channel 19. Also if you press up button from channel 25 you will move to channel 1 and if you press down button from channel 1 you will move to channel 25.<br>There are 13 buttons in the remote as shown in the figure.</p>
<p style="text-align: center;"><img src="./24987/file/c4CJui94.png" alt=""></p>
<p><br>To move to a channel you can press the digits of the channel or you can use Up/Down/Previous buttons. The previous button will take you to the immediately previous channel you watched. (The previous button does not take effect until you have moved to some other channel after the first one.)</p>
<p>The remote control responds to delays. So you can take the button presses "1" and "9" either as a way to go to  channel 1 and then to channel 9, or to channel 19 directly.<br><br>You are given the sequence of channels that the boy wanted to watch.  Find the minimum number of remote button presses required by the boy.  It's not necessary to watch the given channels consecutively, but it is necessary to watch them in the order specified. (In other words, the given sequence must be a subsequence of the optimal channel series the boy chooses to watch.)</p>
<p>To watch the first channel in the sequence, you must press the digits of the channel.</p>
<p><br><strong>Input:</strong></p>
<p>The first line consists of and integer t, the number of test cases. Each test case consists of 4 lines. The first line consists of 2 integers n and k, the number of channels in the remote and the number of channels blocked. The next line consists of k unique integers - the id of the blocked channels. The next line consists of an integer m the number of channels the boy wants to watch followed by a line with m integers - the channel id's of the channels that the boy wants to watch.</p>
<p><strong>Output:</strong></p>
<p>For each test case print the minimum number of remote button clicks required.<br><br><strong>Input Constraints:</strong></p>
<p>1&lt;=t&lt;=100</p>
<p>1&lt;=k&lt;n&lt;=1000</p>
<p>1&lt;=m&lt;=1000</p>
<p>ChannelToWatch[i] != ChannelToWatch[i-1]</p>
<p>ChannelToWatch[any] != BannedChannel[any]</p>
<p><br><strong>Sample Input:</strong></p>
<p>3</p>
<p>5 0</p>
<p>&nbsp;</p>
<p>5</p>
<p>1 2 3 4 5</p>
<p>500 0</p>
<p>&nbsp;</p>
<p>4</p>
<p>140 160 139 160</p>
<p>5 2</p>
<p>2 4</p>
<p>5</p>
<p>1 3 5 3 5<br><br><strong>Sample Output:</strong></p>
<p>Case #1: 5</p>
<p>Case #2: 9</p>
<p>Case #3: 5</p>
<p>&nbsp;</p>
<p><strong>Note:</strong> Suppose you are currently at channel 6 and press up button twice you will move to channel 8. Now if you click on previous button, you will move to channel 7 and not channel 6.<br><br><strong>Exlanation of Case #2</strong>:<br><br>The moves are "1", "4", "0", "down", "1", "6", "0", "previous", "previous"</p>
<p>&nbsp;</p>
<p>Congrats and thanks to <strong><a style="text-decoration: none; color: #0000a0;" href="../../../users/cyclops">Mitch Schwartz</a>&nbsp;</strong>for solving this problem first and for helping on setting test cases for this problem.</p>