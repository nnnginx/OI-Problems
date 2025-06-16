<p align="center"><strong><span style="font-family: verdana, geneva;">Space Bridges</span></strong></p>
<p><span style="font-family: verdana, geneva;">A long time ago, in a galaxy far, far away��. war is going on between the Galactic Empire and the Rebel Alliance. During wars like these, space bridges are really resourceful as they can transfer almost anything including Storm Trooper armies from one space region to another in just mere seconds. Each space region consists of many sectors. The sectors are connected with each other via space roads in such a way that there is exactly one path from one sector to another within a space region. Note that space roads and space bridges are not the same.</span></p>
<p><span style="font-family: verdana, geneva;">The sectors of two space regions of the empire have already been arranged. To find if the arrangement is strong enough, the Supreme&nbsp;<em>Commander</em>&nbsp;of the Imperial Forces has ordered you, their top programmer to calculate the total strength of the two regions.</span></p>
<p style="text-align: center;"><span style="font-family: verdana, geneva;"> <img src="file://Ar8zyCHS.png" alt="graph" width="550px" height="250px"> <br></span></p>
<p><span style="font-family: verdana, geneva;">Two regions can be connected using exactly one Space Bridge from one sector of a region to one sector of the other region. The value of a space bridge connection is the maximum path length you need to travel from any sector of one region to any sector of the other region using any space road or space bridge at most once.<em> </em>The total strength of two regions is the summation of the power of all possible space bridge connections.<em>&nbsp;</em></span></p>
<p><em><span style="font-family: verdana, geneva;">Given the sector arrangements of both space regions, your task is to find the total strength of the two regions. Unfortunately, if the strength isn��t as expected, the Supreme Commander will use his ��Force Choke�� on you, so good luck!</span></em></p>
<p><strong><span style="font-family: verdana, geneva;">Input</span></strong></p>
<p><span style="font-family: verdana, geneva;">Input starts with an integer&nbsp;<strong>T (�� 20)</strong>, denoting the number of test cases.</span></p>
<p><span style="font-family: verdana, geneva;">Each case starts with a line containing two integers&nbsp;<strong>n </strong>and <strong>m (1 �� n,m �� 10<sup>5</sup>)</strong>&nbsp;denoting the number of sectors in the two space regions correspondingly. The next <strong>n-1 </strong>lines denotes the sector arrangement of the first region. Each line will contain <strong>u </strong>and <strong>v (1 &lt;= u,v &lt;= n, u!=v) </strong>denoting that there is a space road connection between the sectors <strong>u </strong>and <strong>v </strong>of the first region. It is guaranteed that the arrangement is such that there will be exactly one path from any sector to another and no same space road will occur twice in the given input. The next <strong>m-1 </strong>lines denotes the sector arrangements of the second region containing <strong>p </strong>and <strong>q (1 &lt;=p,q &lt;= m, p!=q) </strong>which is analogous to the arrangement of the first region.</span></p>
<p><strong><span style="font-family: verdana, geneva;">Output</span></strong></p>
<p><span style="font-family: verdana, geneva;">For each case, in a single line print the case number and the strength of the combined region the space regions.</span></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="319" valign="top">
<p><strong><span style="font-family: verdana, geneva;">Sample Input</span></strong></p>
</td>
<td width="319" valign="top">
<p><strong><span style="font-family: verdana, geneva;">Output for Sample Input</span></strong></p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">2 4</span></p>
<p><span style="font-size: small;">2 1</span></p>
<p><span style="font-family: verdana, geneva;"><span style="font-size: small;">2 3</span></span></p>
<p><span style="font-size: small;">3 1</span></p>
<p><span style="font-size: small;">3 4</span></p>
<p><span style="font-size: small;">2 1</span></p>
<p><span style="font-size: small;">2 1</span></p>
</td>
<td width="319" valign="top">
<p><span style="font-size: small;">Case 1: 30</span></p>
<p><span style="font-size: small;">Case 2: 4</span></p>
</td>
</tr>
</tbody>
</table>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<p><span style="font-family: verdana, geneva;"><span style="text-decoration: underline;"><strong>Note</strong>:</span> In the second sample, there are 2 possible space bridge connections. The first connection is by connecting the first sector of the first region to the first sector of the second region and the second connection is by connecting the second sector of the first region to the first sector of the second region. The values of both the space bridge connections is 2, as you need no more than 2 space roads and space bridges to travel from any sector of the first region to the only sector of the second region. So the total strength is 2+2=4. Look at the figures for better understanding.</span></p>
<p><span style="font-family: verdana, geneva;"><strong>N.B. Dataset is huge, use faster IO</strong></span></p>
<p><span style="font-family: verdana, geneva;"><strong>Problem Setter: Aninda Majumder</strong></span></p>
<p><span style="font-family: verdana, geneva;"><strong>Special Thanks: Momontho Mashak Monmoy, Nafis Sadique, Ahmad Faiyaz</strong></span></p>