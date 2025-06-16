<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MSE08H/en/">English</a></td>
<td width="50%"><a href="/problems/MSE08H/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>&nbsp;</p>
<p>We say that a set S = {x1, x2, ¡­, xn} is factor closed if for any xi ¡Ê S  and any divisor  d of  xi we have d ¡Ê S. Let¡¯s build a GCD matrix  (S) = (sij), where  sij = GCD(xi, xj) ¨C the greatest common divisor  of xi and xj. Given the factor closed set S, find the value of the determinant:</p>
<p><img src="../../../../../../content/simes:MSE08H.jpg" border="0"></p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The input file contains several test cases. Each test case starts  with an integer  n (0 &lt;  n &lt; 1000), that stands for the cardinality  of  S. The next line contains the numbers of S: x1, x2, ¡­, xn. It is known  that each xi is an integer, 0 &lt; xi &lt; 2*10^9. The input data set is  correct and ends with an end of file.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each test case find and print the value Dn mod 1000000007.</p>
<p>&nbsp;</p>
<h3>Sample</h3>
<pre>Input :
2 
1 2 
3 
1 3 9 
4 
1 2 3 6 
Ouput: 
1 
12 
4 
</pre>
<p> </p>