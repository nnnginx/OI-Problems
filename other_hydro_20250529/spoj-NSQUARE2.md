<p><span style="white-space: normal;"><span style="font-size: small;"> </span></span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-size: small;"><strong>N-square Sum! Problem? ( Medium )</strong>&nbsp;</span></p>
<p style="margin-bottom: 0in; text-align: left;"><span style="font-size: small;">Given Q pairs of integers Ni, Ai ( 1 &lt;=  Ai, Q &lt;= 10^5 , 4 &lt;= N &lt;= 10^2 ) a, find Ni numbers whose square sums is equal to Ai. If there're more than one solution, print the one lexicographically smallest . If there's no solution, print "Impossible".</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><br></span></p>
<table style="width: 167px;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="157"> </colgroup> 
<tbody>
<tr>
<td style="border: 1px solid #000000; padding: 0.04in;" width="157" valign="TOP">
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-size: small;">Q 			= 1</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-size: small;">Ni 			= 4</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-size: small;">A1 			= 16</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><br></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-size: small;">{ 4² + 			0² + 0² + 0²  = 16}</span></span></p>
</td>
</tr>
</tbody>
</table>
<p><span style="white-space: normal;"><span style="font-size: small;"><span style="font-size: small;"> </span></span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><br></span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-size: small;"><strong><span style="font-size: small;">Input</span></strong></span></p>
<p style="margin-bottom: 0in; text-align: left;"><span style="font-size: small;">&nbsp;There's an integer Q ( 1 &lt;= Q &lt;= 10^5 ) in the first line; it stands for the number of queries. The next Q lines describe each query with two integers Ni, Ai ( 1 &lt;= Ai &lt;= 10^5, 4 &lt;= Ni &lt;= 10^2 ). Ni is the number of integers that you need to find whose sum of squares is equal to Ai.</span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-size: small;">&nbsp;<strong>Output</strong></span></p>
<p style="margin-bottom: 0in; text-align: left;"><span style="font-size: small;">&nbsp;<span style="text-align: left;">You have to print Q lines, each one with Ni numbers such that the sum of squares is equal to Ai. If there's no solution, you've to print "Impossible".</span></span></p>
<p style="margin-bottom: 0in; text-align: center;"><span style="font-size: small;">&nbsp;<strong>Example</strong></span></p>
<p style="margin-bottom: 0in;" align="CENTER"><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><br></span></p>
<table style="width: 103px;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="93"> </colgroup> 
<tbody>
<tr>
<td style="border: 1px solid #000000; padding: 0.04in;" width="93" valign="TOP">
<p align="LEFT"><span style="font-size: small;"><strong><span style="font-size: small;">Input:</span></strong></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-size: small;">1</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-size: small;">4 16</span></span></p>
<p align="LEFT"><span style="font-size: small;"><strong><span style="font-size: small;">Output:</span></strong></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-size: small;">0 0 0 4</span></span></p>
<p align="LEFT"><span style="font-size: small;"><br></span></p>
<p align="LEFT"><span style="font-size: small;"><strong><span style="font-size: small;">Input:</span></strong></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-size: small;">1</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-size: small;">4 15</span></span></p>
<p align="LEFT"><span style="font-size: small;"><strong><span style="font-size: small;">Output:</span></strong></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-size: small;">1 1 2 3</span></span></p>
<p align="LEFT"><span style="font-size: small;"><br></span></p>
</td>
</tr>
</tbody>
</table>