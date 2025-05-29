<pre><br><span style="white-space: normal;"><p style="margin-bottom: 0in; text-align: center;"><span style="font-family: Arial, sans-serif;"><span style="font-size: medium;"><strong>H-Numbers</strong></span></span>&nbsp;</p><p style="margin-bottom: 0in; text-align: left;"><span style="font-family: Arial, sans-serif; font-size: small; text-align: justify;"><strong>Note: Some tricky testcases were added on Feb. 26th, 2013 and time limit has been changed. All the solutions have been rejudge and some "Accepted" ones got Wron Answer/Time Limit Exceeded. However, this problem can still be solved by a simple and beautiful solution :)</strong></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Ualter is a smart guy, and he loves mathematics and everything related with numbers. Recently his friend Matheus Pheverso showed him a group of H-numbers. Also, his friend told him that, in the Ancient Greek, there h-numbers would be used to create music. This group of numbers can be described in this way:</span></span></p>
<ul>
<li>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">For 	each integer N, a positive integer  A is H-Number with N only if:<br> - LCM(N,A) = N*A</span></span></p>
</li>
<li>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">LCM 	is the Lowest Common Multiple between two numbers.</span></span></p>
</li>
<li>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Ex1: 	N = 20, H-Numbers = {1,3,7,9,11,13,17,19}</span></span></p>
</li>
<li>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Ex2: 	N = 10, H-Numbers = {1,3,7,9}</span></span></p>
</li>
</ul>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Ualter loves classical music mainly Pachelbel's compositions. In order to achieve his old dream, he's willing to make a version of Canon in D using only h-numbers to create notes. </span><span style="color: #333333;"><span style="font-size: small;">To solve that problem, he needs, for each number N, the number of h-numbers of N that are between 1 and M, inclusive.</span></span></span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-family: Arial, sans-serif;"><span style="font-size: medium;"><strong>Task</strong></span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">You're given an integer Q - the number of queries - , and two numbers N,M in each query, your task is to find the number of h-numbers of N between 1 and an integer M.</span></span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-family: Arial, sans-serif;"><span style="font-size: medium;"><strong>Input</strong></span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">In the first line there's an integer Q ( 1 &lt;= Q &lt;= 10^5 ) representing the number of queries. In the next Q lines there're two numbers N,M ( 1 &lt;= N, M &lt;= 10^5 ,  M &lt; N ).</span></span>&nbsp;</p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-family: Arial, sans-serif;"><span style="font-size: medium;"><strong>Output</strong></span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">You have to print for each query an integer xi representing the number of H-numbers of N less  or equal to M.</span></span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-family: Arial, sans-serif;"><span style="font-size: medium;"><strong>Examples</strong></span></span></p>
<p style="margin-bottom: 0in;" align="CENTER">&nbsp;</p>
<table style="width: 97px;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="87"> </colgroup>
<tbody>
<tr>
<td style="border: 1px solid #000000; padding: 0.04in;" width="87" valign="TOP">
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Input:</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">3</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">20 15</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">7 3</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">10 8</span></span></p>
<p align="LEFT">&nbsp;</p>
</td>
</tr>
<tr>
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in;" width="87" valign="TOP">
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">Output:</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">6</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">3</span></span></p>
<p align="LEFT"><span style="font-family: Arial, sans-serif;"><span style="font-size: small;">3</span></span></p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p></span></pre>