<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">Eloy is a hard worker man, however, he is constantly bullied by his superiors, molested by this, one day he was wondering in what ¡°rank¡± you are, so you can bully the people with lower ranks, also to discover who can really bully Eloy!.</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">&nbsp;</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">Now, given the number of employees and the number of relations between them, Eloy need you to output the ¡°rank¡± which employee is in, being 1 the ¡°boss¡± (not bullied by anybody) and the employee who are in these ranks</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">&nbsp;</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">INPUT:</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">There will be an integer T denoting the test cases, then, T test cases will follow, each test case starts with two integers N and R, the number of employees and the number of relations between them, the next R lines consists in two integers R1 and R2, meaning that ¡°employee R1 is lower than employee R2's rank¡±.</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">&nbsp;</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">OUTPUT:</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">You will output for each test case the string ¡°Scenario #i:¡± where i is the test case you are analyzing, after that, you will print N lines, for each line you will output the rank of the employee and the employee itself, if there is the same rank for several employees, then output them lexicographically ordered (the first is the lower)</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">&nbsp;</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">SAMPLE DATA:</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">&nbsp;</span></p>
<table style="width: 100%;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="128*"> <col width="128*"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0.04in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="CENTER"><span style="font-size: large;"><strong><span style="font-size: small;">INPUT</span></strong></span></p>
</td>
<td style="border: 1px solid #000000; padding: 0.04in;" width="50%">
<p align="CENTER"><span style="font-size: large;"><strong><span style="font-size: small;">OUTPUT</span></strong></span></p>
</td>
</tr>
<tr valign="TOP">
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="LEFT"><span style="font-size: small;">2</span></p>
<p align="LEFT"><span style="font-size: x-small;"><br></span></p>
<p align="LEFT"><span style="font-size: small;">5 			6</span></p>
<p align="LEFT"><span style="font-size: small;">2 			0 </span></p>
<p align="LEFT"><span style="font-size: small;">2 			4 </span></p>
<p align="LEFT"><span style="font-size: small;">1 			4 </span></p>
<p align="LEFT"><span style="font-size: small;">1 			2 </span></p>
<p align="LEFT"><span style="font-size: small;">3 			2 </span></p>
<p align="LEFT"><span style="font-size: small;">4 			0 </span></p>
<p align="LEFT"><span style="font-size: small;">&nbsp;</span></p>
<p align="LEFT"><span style="font-size: small;">5 			4 </span></p>
<p align="LEFT"><span style="font-size: small;">1 			0 </span></p>
<p align="LEFT"><span style="font-size: small;">2 			0 </span></p>
<p align="LEFT"><span style="font-size: small;">3 			2 </span></p>
<p align="LEFT"><span style="font-size: small;">4 			2</span></p>
</td>
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in;" width="50%">
<p align="LEFT"><span style="font-size: small;">Scenario 			#1: </span></p>
<p align="LEFT"><span style="font-size: small;">1 			0 </span></p>
<p align="LEFT"><span style="font-size: small;">2 			4 </span></p>
<p align="LEFT"><span style="font-size: small;">3 			2 </span></p>
<p align="LEFT"><span style="font-size: small;">4 			1 </span></p>
<p align="LEFT"><span style="font-size: small;">4 			3 </span></p>
<p align="LEFT"><span style="font-size: small;">Scenario 			#2: </span></p>
<p align="LEFT"><span style="font-size: small;">1 			0 </span></p>
<p align="LEFT"><span style="font-size: small;">2 			1 </span></p>
<p align="LEFT"><span style="font-size: small;">2 			2 </span></p>
<p align="LEFT"><span style="font-size: small;">3 			3 </span></p>
<p align="LEFT"><span style="font-size: small;">3 			4</span></p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in;" align="LEFT">&nbsp;</p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">"Blank line between test cases for clarification and separation"&nbsp;</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">"Please note that can be more than one "boss" (not bullied by anybody)"</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: large;"><strong><span style="font-size: small;">CONSTRAINTS:</span></strong></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: large;"><em><span style="font-size: small;">1&lt;=N&lt;=1000; 1&lt;=R&lt;=10000</span></em></span></p>