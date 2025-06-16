<p>Tanmoy recently learn about euclid gcd algorithm.</p>
<p>This algorithm looks like:</p>
<p>gcd(a,b):</p>
<p>&nbsp;&nbsp; if(b==0):return a</p>
<p>&nbsp;&nbsp; return gcd(b,a%b)</p>
<p>Now he want to find out how many pair (x,y) can be possible in range N, which gcd is greater than 1. Here pair (x,y) and (y,x) consider as same pair. 1&lt;=x,y&lt;=N.</p>
<p>He can find out it small number easily but for a large number its realy hard to find out. Now he needs your help. Write a programme that find out number of such pair.</p>
<p><strong>Input:</strong><strong>&nbsp;</strong></p>
<p>Input start with an integer number T(¡Ü10^5), which is number of test cases.</p>
<p>Each test case contain a integer N (1¡ÜN¡Ü10^5).</p>
<p><strong>Output:</strong></p>
<p>For each case, Print case Number and Desired answer</p>
<p><strong>Sample: </strong></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="138" valign="top">
<p>Input</p>
</td>
<td width="480" valign="top">
<p>Output</p>
</td>
</tr>
<tr>
<td width="138">
<p>2<br>3<br>4</p>
<p>&nbsp;</p>
</td>
<td width="480">
<p>Case 1: 2<br>Case 2: 4</p>
</td>
</tr>
</tbody>
</table>
<p><strong><span style="text-decoration: underline;">&nbsp;</span></strong></p>