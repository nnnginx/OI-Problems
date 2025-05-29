<pre><span style="white-space: normal;"><span style="font-family: verdana, geneva;"><p>Making a fun is a not a bad thing, but while making a fun if you disrespect someone then it will not be acceptable. Some of the North South University's students has done this type of wrong thing. So as a punishment they have to solve this problem. And you are a friend of them, so you should help them.</p>
<p>&nbsp;</p>
<p>You will have N segments. Each one is connected in contiguous way. And we can number them from 1 to N. See the following figure:</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img title="figure" src="file://Bgi1Cwwc.png" alt="figure" width="808" height="70"></p>
<p>&nbsp;</p>

<p>&nbsp;</p><p>Now you need to paint them, you have some colors, which are numbered from 1 to M. Now you need to count number of ways to paint the segments with the colors, such that this property preserves-</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; U = color(i) + color(j)</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; V = color(j) + color(k)</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; U, V is Coprime.</p><p><span style="white-space: pre;">	</span>&nbsp; &nbsp; Here <strong>1 &lt;= i &lt; j &lt; k &lt;= N</strong> and j = i + 1, k = j + 1</p>
<p>And i, j, k indicates the index of segments and color(i) means the color you have painted on i th segment.</p>
<p><strong>&nbsp;</strong></p>
<p><strong>Input</strong></p>
<p>Input starts with an integer&nbsp;<strong>T (�� 2500)</strong>, denoting the number of test cases.</p>
<p>Each case starts with a line containing two integers&nbsp;<strong>N</strong>, <strong>M.</strong></p>
<p>&nbsp;1 &lt;= N &lt;= 50</p><p>&nbsp;1 &lt;= M &lt;= 50</p>
<p><strong>Output</strong></p>
<p>For each case, print the case number and the number of ways to paint the segments following above conditions. Since the result can be very large, you have to print the result modulo&nbsp;<strong>1000003</strong></p>
<table border="1" cellspacing="0" cellpadding="0">
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
<p>3</p>
<p>3 1</p>
<p>3 2</p>
<p>3 3</p>
<p>&nbsp;</p>
</td>
<td width="319" valign="top">
<p>Case 1: 0</p>
<p>Case 2: 4</p>
<p>Case 3: 14</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p></span></span></pre>