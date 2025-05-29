<p>Mr. Bean loves to play games. For this he wastes lots of money so Mrs.Bean made a hurdle game for him. Now in the game we have 3 tracks and for moving up to next level he will have to cross some hurdles.Each time he changes the track he gets some drink to increase his energy level by that amount.The drink that he gets is the one which is in between the present track and the adjacent track and in the direction of movement (adjacent track may or may not be the track on which he is targetting to move).Now if at any moment his energy becomes negative his game will be over. So you have make him win this game with maximum energy being available with him at last. He will move in the form of 'L' and 'R' between adjacent tracks with 'L' making him move one step left of the present position and 'R' moving him right. Movement between different level will be seperated by '-' and if their is no change of track between adjacent levels then print 'U' at its corresponding move .</p>
<pre><a href="http://tinypic.com?ref=c3o8w" target="_blank"><img src="../../../../../../content/simes:BEANGAME.jpg" border="0" alt="Image and video hosting by TinyPic"></a></pre>
<h3>Input</h3>
<p>First line will have 3 integers Il,Ie,Ns where Il is the initial track on which he is standing, Ie is the initial<br>energy he is having and Ns is the number of levels in the game.<br>Then it would be followed by 5 lines where the first three will have the values of the hurdles present at each level<br>on each track.Fourth line will have Ns-1 integers representing the energy obtained by him on drinking the energy<br>drink between continuous levels between track 1 and 2 and similarly fifth line will have Ns-1 values for drinks between<br>tracks 2 and 3.</p>
<h3>Output</h3>
<p>Print "DONE IT!" in first line and the steps taken by him in second line following the path which leads to maximum energy available with Mr.Bean beyond final track.<br>If it is not possible print "GAME OVER!".</p>
<p>&nbsp;</p>
<p>CONSTRAINTS</p>
<p>Every integer , intermediate values will fit in 32-bit integer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 6 5<br>3 2 9 16 3<br>4 0 7 26 1<br>1 7 3 30 9<br>8 19 8 3<br>10 3 6 4

<strong>Output:</strong>
DONE IT!<br>RR-LL-RR-LL-R
</pre>