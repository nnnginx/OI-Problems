<p><strong><span style="color: #339966;">Bad XOR | BADXOR</span></strong></p>
<p><strong><span style="color: #3366ff;">Time Limit: 1s</span></strong></p>
<p><span style="font-family: verdana, geneva;">You are given an array A of N elements. Also you are given another array B of M elements. Any subset (i­<sub>1</sub>, i<sub>2</sub>, i<sub>3</sub>, …., i<sub>p </sub>) is bad IFF ( Ai<sub>1</sub> ⊕ Ai<sub>2</sub> ⊕ …. ⊕ Ai<sub>p </sub>) equals any value of B. ⊕ means Bitwise XOR, which can be found with ^ syntax in popular programming languages. Now your job is to find the number of good subsets. Empty Subset has XOR value of 0.</span></p>
<p><span style="font-family: verdana, geneva;">&nbsp;</span></p>
<p><strong><span style="color: #339966;">Input</span></strong></p>
<p><span style="font-family: verdana, geneva;">The first line of input denotes the number of test cases T (1 &lt;= T &lt;= 20). The first line of each test case contains two integers N and M ( 0 &lt;= N, M &lt;= 1000). The next line contains N integers of the array A (0 &lt;= A<sub>i </sub>&lt;=1000). The next line contains M integers of the array B (0 &lt;= B<sub>i </sub>&lt;=1000). You can assume that each element of array B will be unique. &nbsp;</span></p>
<p><span style="font-family: verdana, geneva;">&nbsp;</span></p>
<p><strong><span style="color: #339966;">Output</span></strong></p>
<p><span style="font-family: verdana, geneva;">For each case, print the case number and the total numbers of good subsets in a line. As the result can be very big, output it modulo 100000007.</span></p>
<p><span style="font-family: verdana, geneva;">&nbsp;</span></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="332" valign="top">
<p><span style="font-family: verdana, geneva;"><span style="font-family: verdana, geneva;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span><strong><span style="color: #339966;">Sample Input</span></strong></span></p>
</td>
<td width="332" valign="top">
<p align="center"><strong><span style="color: #339966;">Output for   Sample Input</span></strong></p>
</td>
</tr>
<tr>
<td width="332" valign="top">
<p><span style="font-size: small;">2</span></p>
<p><span style="font-size: small;">2 3</span></p>
<p><span style="font-size: small;">1 2</span></p>
<p><span style="font-size: small;">0 1 2</span></p>
<p><span style="font-size: small;">1 3</span></p>
<p><span style="font-size: small;">1</span></p>
<p><span style="font-size: small;">0 1 2</span></p>
</td>
<td width="332" valign="top">
<p><span style="font-size: small;">Case 1: 1</span></p>
<p><span style="font-size: small;">Case 2: 0</span></p>
<p><span style="font-size: small;">&nbsp;</span></p>
</td>
</tr>
</tbody>
</table>
<p><span style="font-family: verdana, geneva;">&nbsp;</span></p>
<p><span style="font-size: medium;">&nbsp;Problem Setter: Nafis Sadique</span></p>
<p><span style="font-size: medium;">Special Thanks: Ahmad Faiyaz</span></p>