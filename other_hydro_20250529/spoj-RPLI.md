<p style="margin-bottom: 0in;">&nbsp;Luis is seeing his son playing, he ask him gently in what the game consists, the boy replies ¡°Its like this, you have a big number, a bound and a ¡°mod¡± (the remainder of a division between a number and ¡°mod¡±), the goal of the game is to discover the maximum sub-number you can create following this rules:¡±</p>
<ul>
<li>
<p style="margin-bottom: 0in;">The sequence must not decrease lower from the first digit taken.</p>
</li>
<li>
<p style="margin-bottom: 0in;">The sequence chosen must <em>not</em> reach the bound. By example, if the first digit is 'd' and a bound 'k', the range you can take is between [d,min(d+k,9)]</p>
</li>
<li>
<p style="margin-bottom: 0in;">You can start from <em>any</em> digit of a number.</p>
</li>
<li>For any given start point, you should look for the sub-numbers making the maximum sum applied to the mod operation.</li>
</ul>
<p style="margin-bottom: 0in;">Luis, astonished by the explanation, request his son to give him and example, the boy then continues: ¡°Suppose a number like this: 56789, a bound of 2, and a mod 10. you start with 5, being the bound of 2, this mean you can take up to the digit 7 (this means that you can always collect as many fives, sixes and sevens following the rules explained). The sub-number formed is of ¡°5+6+7¡±, following the rules, we will have all others sub-numbers: ¡°6+7+8¡± ¡°7+8+9¡± ¡°8+9¡± and ¡°9¡±, after applying the operation, you will find that the maximum remainder of the sub-number's sum will be of ¡°9¡±, made by the sub-number ¡°9¡±.</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;">Luis is a former programmer now and he does not have the same ability he had years ago, please, help him in his task following the game previously defined.</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><strong>INPUT:</strong></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">The first line of input will contain an integer T denoting the T test cases, then, T cases will follow. Each of the following cases will contain a line with an integer L, a big number N in the range [10^(L-1),(10^L)-1], an integer K denoting the bound and the M that will be the mod of the whole operation.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><strong>OUTPUT:</strong></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">Output the string ¡°Scenario #i: ¡° where i is the test case you are analyzing followed by the maximum sum of the sub-sequence that can be formed.</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;">SAMPLE DATA:</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<table style="width: 100%;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="128*"> <col width="128*"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0.04in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="CENTER"><strong>INPUT</strong></p>
</td>
<td style="border: 1px solid #000000; padding: 0.04in;" width="50%">
<p align="CENTER"><strong>OUTPUT</strong></p>
</td>
</tr>
<tr valign="TOP">
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p>4</p>
<p>7 1235678 2 10</p>
<p>7 1235678 2 3</p>
<p>3 679 2 20</p>
<p>4 3457 2 10</p>
</td>
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in;" width="50%">
<p>Scenario #1: 8</p>
<p>Scenario #2: 2</p>
<p>Scenario #3: 16</p>
<p>Scenario #4: 9</p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><strong>CONSTRAINTS:</strong></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">1&lt;=L&lt;=100000</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">10^(L-1)&lt;=N&lt;(10^L)-1</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">1&lt;=K&lt;=8</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">1&lt;=M&lt;=45</p>