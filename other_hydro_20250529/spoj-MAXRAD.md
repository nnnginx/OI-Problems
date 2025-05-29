<p><strong>Maximum Radius | MAXRAD</strong></p>
<p><strong>Time Limit: 2 seconds</strong></p>
<p>You will be given some 2D points. You need to draw circles with each point considering as a center of a circle with minimum radius <strong>1</strong>. And no two drawn circles should intersect with each other or contain each other. Now you have to find the maximum radius any circle can have so that all the circles have radius greater or equal to 1 and no two circles intersect with each other or contain each other. You have to print the maximum radius. If it is not possible to maintain the restriction for any radius, then you should print <strong>-1.000000</strong>.</p>
<p><strong>Input</strong></p>
<p>Input starts with an integer&nbsp;<strong>T (¡Ü 50)</strong>, denoting the number of test cases.</p>
<p>Each case starts with a line containing an integer&nbsp;<strong>N (2 ¡Ü N ¡Ü 1000)</strong>&nbsp;denoting the number of 2D points. Each of the next&nbsp;<strong>N</strong>&nbsp;lines contains two integers&nbsp;<strong>x<sub>i</sub>&nbsp;y<sub>i</sub></strong>&nbsp;<strong>(-10<sup>4</sup>&nbsp;¡Ü x<sub>i</sub>, y<sub>i</sub>&nbsp;¡Ü 10<sup>4</sup>)</strong>&nbsp;denoting the co-ordinate of a point. These points may not be distinct.</p>
<p><strong>Output</strong></p>
<p>For each case, print the maximum radius a circle can have. If it is not possible to maintain the restriction then you should print <strong>-1.000000</strong>. Errors less than&nbsp;<strong>10<sup>-6</sup></strong>&nbsp;will be ignored.</p>
<table border=".5" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="319" valign="top">
<p><strong>Sample Input</strong></p>
</td>
<td width="319" valign="top">
<p><strong>Output for Sample Input</strong></p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">1 1</span></p>
<p><span style="font-size: small;">3 1</span></p>
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">1 1</span></p>
<p><span style="font-size: small;">2 1</span></p>
</td>
<td width="319" valign="top">
<p><span style="font-size: small;">1.000000</span></p>
<p><span style="font-size: small;">-1.000000</span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>Problem Setter: Ahmad Faiyaz</p>
<p>Special Thanks: Aninda Majumder</p>