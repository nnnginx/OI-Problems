<p>&nbsp;</p>
<p>   </p>
<table style="width: 100%; background-color: #44c23c;" border="0">
<tbody>
<tr>
<td style="text-align: center;" width="50%"><a href="%7B$base%7Dproblems/%7B$code%7D/en/">English</a></td>
<td style="text-align: center;" width="50%"><a href="%7B$base%7Dproblems/%7B$code%7D/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Imagine a 2D diagram drawn in the following way: Starting at the origin, you’re given a sequence of letters which is entirely made of the following four letters ’U’, ’D’, ’L’,and ’R’.A ’U’ is an instruction for you to move one unit upward and drawing a segment at the same time. Similarly, ’D’ is for moving down, ’L’ for left, and ’R’ for right.</p>
<p>For example, ﬁgure (a) is drawn by giving the sequence ’UURDLL’ while ﬁgure (b) is the result of ’UURRRDLLLLUURRRDDD’ (in both ﬁgures, the starting point is identiﬁed by a small circle.)</p>
<p><br>While segments are allowed to intersect, they’re not allowed to overlap. In other words, any two segments will have, at most, one point in common. We’re interested in knowing the number of closed polygons, not containing any lines inside, in such diagrams. Figure (a), has only one closed polygon while ﬁgure (b) has three. Write a program to do exactly that.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img src="../../../content/simes:ANARC05I.png" alt=""></p>
<h1 style="text-align: center;">Input</h1>
<p>Your program will be tested on one or more test cases. Each test case is speciﬁed on a separate line. The diagram is speciﬁed using a sequence made entirely of (U|D|L|R) and terminated by the letter ’Q’. All letters are capital letters. None of the segments in a test case will overlap.</p>
<p><br>The end of test cases is identiﬁed by the letter ’Q’ on a line by itself.</p>
<p>Length of each sequence is smaller than 1000.</p>
<h1 style="text-align: center;">Output</h1>
<p>For each test case, write the answer on a separate line.</p>
<h1 style="text-align: center;">Sample</h1>
<pre style="text-align: justify;">input<br>UURDLLQ<br>UURRRDLLLLUURRRDDDQ<br>Q<br><br>output<br>1<br>3</pre>
<p> </p>