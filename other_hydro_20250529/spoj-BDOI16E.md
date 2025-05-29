<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p style="text-align: left;"><span style="font-size: large;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <a name="page1"></a> <span style="color: #00000a;"><strong>Village Fair</strong></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-bottom: 0in; line-height: 106%" align="JUSTIFY"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;">There are N houses in a village far away from here. They are numbered from 1 to N. For this problem lets assume, the houses each can accommodate infinite amount of people. </span><span style="color: #00000a;"><strong>From each house there is a</strong></span><span style="color: #00000a;"> </span><span style="color: #00000a;"><strong>directed path to exactly one other house</strong></span><span style="color: #00000a;">. One of the houses is a grand house. There is a fair going on</span><span style="color: #00000a;"><strong> </strong></span><span style="color: #00000a;">currently in the grand house. From this house there is no exit, and everybody can enjoy the festival here. Initially there is a little kid in each of the houses of the village. Each kid has some non-negative amount of joy(they are all pretty excited about the fair). It is guaranteed that there is exactly one simple way from each house to the grand house.</span></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-right: 0.01in; margin-bottom: 0in; line-height: 141%" align="JUSTIFY"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;">Every kid from their house starts their journey to the grand house. When they go from a house to some other house, their joy changes by some positive or negative amount. This change depends on the path.</span></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-bottom: 0in; line-height: 105%" align="JUSTIFY"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;">Now, for each houses, you have to count the number of distinct joy values that will come to this house at some point of time. Note that if two or more persons with the same joy value will be counted only once. See the sample explanation for details.</span></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-bottom: 0in;"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;"><strong>Input:</strong></span></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-bottom: 0in; line-height: 102%" align="JUSTIFY"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;">You are given an integer N in the first line. The next line will contain N integers, the initial joy value of the kids in the houses. The next line also contains N integers, where the kth integer is the id of the house where the kids can go to from the kth house or 0 if it is the grand house. The fourth line will contain N integers, the amount of change of joy that will occur if one person goes through the path from starting at kth house or 0 if it is the grand house.</span></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-bottom: 0in;"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;"><strong>Output:</strong></span></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-right: 0.01in; margin-bottom: 0in; line-height: 111%" align="JUSTIFY"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;">Print N lines, each containing the number of distinct joy values that will come to this house at some point of time.</span></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p><span style="font-size: small;"> </span></p>
<table style="width: 637px;" border="0" cellspacing="0" cellpadding="7">
<colgroup><col width="292"></colgroup><colgroup><col width="315"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border: 1px solid #4c4c4c; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="292">
<p><span style="font-family: times new roman,times;"><span style="font-size: small;">Input</span></span></p>
</td>
<td style="border: 1px solid #4c4c4c; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="315">
<p><span style="font-family: times new roman,times;"><span style="font-size: small;">Output</span></span></p>
</td>
</tr>
<tr valign="TOP">
<td style="border: 1px solid #4c4c4c; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="292">
<p style="margin-bottom: 0in;"><span style="font-family: times new roman,times;"><span style="font-size: small;">5</span></span></p>
<p style="margin-bottom: 0in"><span style="font-family: times new roman,times;"><span style="font-size: small;">7 3 2 5 1 </span></span></p>
<p style="margin-bottom: 0in"><span style="font-family: times new roman,times;"><span style="font-size: small;">0 1 1 3 3 </span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;">0 4 1 0 4 </span></span></p>
</td>
<td style="border: 1px solid #4c4c4c; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="315">
<p style="margin-bottom: 0in;"><span style="font-family: times new roman,times;"><span style="font-size: small;">3</span></span></p>
<p style="margin-bottom: 0in;"><span style="font-family: times new roman,times;"><span style="font-size: small;">1</span></span></p>
<p style="margin-bottom: 0in;"><span style="font-family: times new roman,times;"><span style="font-size: small;">2</span></span></p>
<p style="margin-bottom: 0in;"><span style="font-family: times new roman,times;"><span style="font-size: small;">1</span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;">1</span></span></p>
</td>
</tr>
</tbody>
</table>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-bottom: 0in;"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;"><strong>Explanation of Sample:</strong></span></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-bottom: 0in; line-height: 88%" align="JUSTIFY"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;">Initially each house will contain the kids with joy { 7, 3, 2, 5, 1 }. The first kid always stays in the grand house. The second kid will go to the grand house with joy 7. The 3</span><span style="color: #00000a;"><sup>rd</sup></span><span style="color: #00000a;"> kid will go to the grand house with joy 3. The fourth kid will go to 3</span><span style="color: #00000a;"><sup>rd</sup></span><span style="color: #00000a;"> house with joy 5 and from there he will make it to grand house with 6 joy. Same goes for 5</span><span style="color: #00000a;"><sup>th</sup></span><span style="color: #00000a;"> person.</span></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-bottom: 0in; line-height: 111%" align="JUSTIFY"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;">So the first house will see { 7, 7, 3, 6, 6}. The second house will see {3}. The third house will see {2, 5, 5} The fourth house will see { 5 } and the fifth house will see { 1 }.</span></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-bottom: 0in;"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;">So the number of distinct joy values of each house is { 3, 1, 2, 1, 1}.</span></span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p><span style="font-family: times new roman,times;"><span style="font-size: small;"> </span></span></p>
<p class="western" style="margin-bottom: 0in;"><span style="font-family: times new roman,times;"><span style="font-size: small;"><a name="_GoBack"></a><span style="color: #00000a;">Limits: Easy(1 &lt;= N &lt;= 1000), Hard(1 &lt;= N &lt;= 100000).</span></span></span></p>
<p class="western" style="margin-bottom: 0in;"><span style="font-family: times new roman,times;"><span style="font-size: small;"><span style="color: #00000a;"><br></span><span style="font-size: medium;"><span style="color: #00000a;"><strong>Problem Setter: Nafis Sadique</strong></span></span></span></span></p>
<p><span style="font-size: small;"> </span></p>