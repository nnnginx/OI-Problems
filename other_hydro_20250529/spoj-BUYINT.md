<p><strong><span style="font-family: verdana, geneva;">Buying Integers</span></strong></p>
<p><strong><span style="font-family: verdana, geneva;">&nbsp;</span></strong></p>
<p><span style="font-family: verdana, geneva;">Let's assume that you have <strong>n</strong> integers, <strong>A<sub>1,</sub> A<sub>2,</sub> A<sub>3</sub> </strong>¡­<strong> A<sub>n </sub></strong></span></p>
<p><span style="font-family: verdana, geneva;">&nbsp;</span></p>
<p><span style="font-family: verdana, geneva;">Let's define,</span></p>
<p><span style="font-family: verdana, geneva;">&nbsp;</span></p>
<p><span style="font-family: verdana, geneva;"><strong>E = </strong>Number of pairs <strong>(i,j)</strong> such that <strong>i&lt;j</strong> and <strong>( A<sub>i </sub>+<sub> </sub>A<sub>j </sub>) </strong>are even .<strong></strong></span></p>
<p><span style="font-family: verdana, geneva;"><strong>O</strong> <strong>=</strong> Number of pairs <strong>(i,j)</strong> such that <strong>i&lt;j</strong> and <strong>( A<sub>i </sub>+<sub> </sub>A<sub>j </sub>)</strong> are odd .<strong></strong></span></p>
<p><strong><span style="font-family: verdana, geneva;">D = | E-O |</span></strong></p>
<p><strong><span style="font-family: verdana, geneva;">&nbsp;</span></strong></p>
<p><span style="font-family: verdana, geneva;">That means, <strong>D = (E-O) </strong>if <strong>(E-O) </strong><strong>¡Ý 0 , -(E-O) </strong>otherwise .</span></p>
<p><span style="font-family: verdana, geneva;">&nbsp;</span></p>
<p><span style="font-family: verdana, geneva;">Unfortunately, you do have <strong>n </strong>but those <strong>n</strong> integers are lost . You will have to buy them again. Before going to the market, you have decided that you will buy <strong>n</strong> integers in such a way that the value of <strong>D </strong>will be as small as possible, as you will have to pay <strong>D </strong>golden coins, to buy them.</span></p>
<p><span style="font-family: verdana, geneva;">&nbsp;</span></p>
<p><span style="font-family: verdana, geneva;">Now,you are wondering, what that minimum <strong>D [</strong>Let's say it <strong>D<sub>min</sub>] </strong>will<strong> </strong>be<strong> </strong>.</span></p>
<p><span style="font-family: verdana, geneva;">&nbsp;</span></p>
<p><strong><span style="font-family: verdana, geneva;">Input</span></strong></p>
<p><strong><span style="font-family: verdana, geneva;">&nbsp;</span></strong></p>
<p><span style="font-family: verdana, geneva;">First line of the input file will contain the number of test cases, <strong><strong>T ¡Ü 1000000</strong></strong>, followed by <strong>T </strong>lines, each containing an integer <strong>n</strong> (<strong>1 </strong>¡Ü <strong>n </strong>¡Ü <strong>10<sup>9</sup>) </strong>.</span></p>
<p><span style="font-family: verdana, geneva;">&nbsp;</span></p>
<p><strong><span style="font-family: verdana, geneva;">Output</span></strong></p>
<p><strong><span style="font-family: verdana, geneva;">&nbsp;</span></strong></p>
<p><span style="font-family: verdana, geneva;">For each case, print the case number starting from 1 and <strong>D<sub>min </sub></strong>for the value of <strong>n </strong>in that particular case. See the sample output for exact formatting.<strong></strong></span></p>
<p><strong><span style="font-family: verdana, geneva;">&nbsp;</span></strong></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="278" valign="top">
<p align="center"><strong><span style="font-family: verdana, geneva;">Sample Input</span></strong></p>
</td>
<td width="333" valign="top">
<p align="center"><span style="font-family: verdana, geneva;"><strong>Output for Sample   Input</strong><strong></strong></span></p>
</td>
</tr>
<tr>
<td width="278" valign="top">
<p><span style="font-family: verdana, geneva;">3</span></p>
<p><span style="font-family: verdana, geneva;">3</span></p>
<p><span style="font-family: verdana, geneva;">4</span></p>
<p><span style="font-family: verdana, geneva;">5</span></p>
</td>
<td width="333" valign="top">
<p><span style="font-family: verdana, geneva;">Case   1:   1</span></p>
<p><span style="font-family: verdana, geneva;">Case   2:   0</span></p>
<p><span style="font-family: verdana, geneva;">Case   3:   2</span></p>
</td>
</tr>
</tbody>
</table>
<p><strong>Warning</strong> : Input file is huge, please use faster input and output methods (e.g. printf and scanf in C++) .</p>
<p>Problem Setter: Momontho Mashak Monmoy</p>
<p>Special Thanks: Muhammad Ridowan</p>