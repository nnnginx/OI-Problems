<h3>  Piece it together</h3>
<!--l. 3-->
<p>Tom has developed a special kind of puzzle: it involves a whole bunch of identical puzzle pieces. The pieces have the shape of three adjoint squares in an L-shape. The corner square is black, the two adjacent squares are white. <!--l. 8--></p>
<p>&nbsp;</p>
<hr>
<div id="x1-10011"><!--l. 10-->
<p></p><center><img src="/NWERC11/content/problemD0x.png" alt="PIC" width="86.32251pt" height="86.32251pt"></center><!--tex4ht:graphics   name="/NWERC11/content/problemD0x.png" src="puzzlepiece.eps"   --><p></p>
<div>Figure&nbsp;1: A puzzle piece</div>
<!--tex4ht:label?: x1-10011 --> <!--l. 12-->
<p>&nbsp;</p>
</div>
<hr>
<!--l. 14-->
<p>The puzzler is given a pattern of black and white squares in a rectangular grid. The challenge is to create that pattern using these pieces. The pieces can be rotated, but must not overlap. <!--l. 18--></p>
<p>Tom has already designed a few nice patterns, but he needs to find out if they can be constructed with the pieces at all. Rather than trying to test this for each pattern by hand, he wants to write a computer program to determine this for him. Can you help him?</p>
<h4>Input</h4>
<!--l. 24-->
<p>On the first line a positive integer: the number of test cases, at most 100. After that per test case:</p>
<ul>
<li>one line with two integers <em>n </em>and <em>m </em>(1 ¡Ü <em>n,m </em>¡Ü 500): the height and width of the       grid containing the pattern, respectively. </li>
<li><em>n </em>lines, each containing <em>m </em>characters, denoting the grid. Each character is ¡®<tt>B</tt>¡¯, ¡®<tt>W</tt>¡¯, or       ¡®<tt>.</tt>¡¯, indicating a black, white or empty square respectively.</li>
</ul>
<!--l. 34-->
<p>The grid contains at least one black or white square. <!--l. 36--></p>
<p>&nbsp;</p>
<h4>Output</h4>
<!--l. 37-->
<p>Per test case:</p>
<ul>
<li>one line with either ¡°<tt>YES</tt>¡± or ¡°<tt>NO</tt>¡±, indicating whether or not it is possible to construct       the pattern with the puzzle pieces. You may assume that there is an infinite supply       of pieces.</li>
</ul>
<!--l. 44-->
<p>&nbsp;</p>
<h4>Sample in- and output</h4>
<table align="center" id="TBL-1" border="1" cellspacing="5" cellpadding="5" rules="groups">
<colgroup><col id="TBL-1-1"></colgroup><colgroup id="TBL-1-2g"><col id="TBL-1-2"></colgroup>
<tbody>
<tr id="TBL-1-1-" style="vertical-align:baseline;">
<td id="TBL-1-1-1" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Input</span></p>
</td>
<td id="TBL-1-1-2" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Output</span></p>
</td>
</tr>
<tr id="TBL-1-2-" style="vertical-align:baseline;">
<td id="TBL-1-2-1" style="white-space:wrap; text-align:left;"><!--l. 46-->
<pre>2
3 4
BWW.
WWBW
..WB
3 3
W..
BW.
WBW</pre>
</td>
<td id="TBL-1-2-2" style="white-space:wrap; text-align:left;"><!--l. 50-->
<pre>YES
NO </pre>
</td>
</tr>
</tbody>
</table>
<h4>Copyright notice</h4>
<p>
This problem text is copyright by the NWERC 2011 jury. It is
licensed under the Creative Commons Attribution-Share Alike license
version 3.0; The complete license text can be found at:
<a href="http://creativecommons.org/licenses/by-sa/3.0/legalcode">http://creativecommons.org/licenses/by-sa/3.0/legalcode</a>
</p>