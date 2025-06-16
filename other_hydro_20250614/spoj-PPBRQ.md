<p><a href="http://contest.bayan.ir/en/contest/qualification_2014/problem/C/">Main Problem Source</a><br><br>The Farfaraway planet is an extraterrestrial one. Recent astronomers' researches show that this planet is cube-shaped, and a word is written on each side of the cube. Also this weird planet has 3 types of rotations around&nbsp;<strong>3 axises</strong>. Those are:</p>
<p><strong>Rotation of type X:</strong>&nbsp;Right and left sides remain still, and the cube turns upward.</p>
<p><img src="./23946/file/ZaGKIn9V.png" alt=""></p>
<p><strong>Rotation of type Y:</strong>&nbsp;Front and rear sides remain still, and the cube turns toward right.</p>
<p><img src="./23946/file/WmihJdlY.png" alt=""></p>
<p><strong>Rotation of type Z:</strong>&nbsp;Top and bottom sides remain still, and the cube turns toward right.&nbsp;</p>
<p><img src="./23946/file/ASGbaeib.png" alt=""></p>
<p>Given a cube with some words written on its each side and a sequence of rotations, you should determine the word on each cube side.</p>
<p><img src="./23946/file/TNosUsvP.png" alt=""></p>
<p align="center">&nbsp;</p>
<p><strong>Input</strong></p>
<p>First line of input contains an integer&nbsp;<strong>T</strong>, denoting number of testcases.</p>
<p>In each testcase First line contains six words (consisting of english letters, and not longer than 10 characters), which are the initial words on Front, Top, Bottom, Left, Right, and Rear side of the cube. Second line contains a number N, number of rotation sequences. Next&nbsp;<strong>N</strong>&nbsp;line contain a character&nbsp;<strong>X, Y</strong>&nbsp;or&nbsp;<strong>Z</strong>&nbsp;indicating type of the rotation, followed by&nbsp;<strong>m</strong>&nbsp;indicating that rotation was performed m times.</p>
<p>Here,&nbsp;<strong>1&lt;=T&lt;=1000</strong>,&nbsp;<strong>1&lt;=N&lt;=100000</strong>,&nbsp;<strong>1&lt;=m&lt;=10^9</strong>.</p>
<p><strong>&nbsp;</strong></p>
<p><strong>Output</strong></p>
<p>For each testcase, output the words on Front, Top, Bottom, Left, Right, and Rear side after applying those rotations.</p>
<p><strong>Sample test(s)</strong></p>
<p><strong>input</strong></p>
<p>2<br> Front Up Down Left Right Back<br> 2<br> Z 4<br> X 4<br> Front Up Down Left Right Back<br> 3<br> Z 1<br> X 1<br> Y 1</p>
<p><strong>output</strong></p>
<p>Front Up Down Left Right Back<br> Down Back Front Right Left Up</p>
<p><strong>input</strong></p>
<p>1<br> a b c d e f<br> 3<br> X 5<br> Y 5<br> Z 5</p>
<p><strong>output</strong></p>
<p>f d e b c a</p>
<p>&nbsp;</p>