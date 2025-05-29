<p style="margin-bottom: 0in;" align="JUSTIFY"><span lang="en-US">The female Alien moved to the biggest city in the world, this city has a giant subway system, this subway is always full of people, the Alien doesn't want to see humans and she wants to stay the least time possible in the subway system.</span></p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">Preventing this scenario, the Alien brought from her planet some interesting and very rare objects, she calls this objects ��Portable Teleporters��, with these objects the alien is on the capacity to teleport and ignore the next K stations, as you may know, this objects are limited and it can be used once.</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">As the city is so big that the subway is always full, she wants to stay the least number stations as possible, the Alien will start from station 0, wishing to go up to an station L, the subway is formed by N+1 (0 through N) stations and the Alien has K ��Portable Teleporters��.</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">When the Alien uses a ��Portable Teleporters�� she will be teleported immediately to the I+Kj station, being I the station the alien was on and Kj the value of the Portable Teleporter.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span lang="en-US"> If she is unable to use a teleporter or is better for her to go into the next station using the subway, she can do it, however, she can onl</span><span lang="en-US">y move forward, NEVER backwards, furthermore, the Alien may not leave the limits of the stations (that means she can't go to any station before station 0 or any station after station N).</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span lang="en-US">&nbsp;</span>As you may know, the Alien doesn't wants to see a large number of people, to prevent this, she wants to visit as maximum T stations, if she can't reach her destination on T stations, she will simply exit the subway and will start walking on the city.</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">Your task is simple, given the N stations, the K objects and their values and the station the Alien wants to go, the L station the alien wants to go and the T number of tries,&nbsp;output the least stations visited so she can reach her destination.</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span lang="en-US"><strong>INPUT</strong></span><span lang="en-US">:</span></p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">The Input will start with an integer P denoting the test cases, then P cases will follow, each case have three lines, the first line contains two integers N and K, denoting the N stations and the K portable teleporters, next line will contain K integers, denoting the value of each teleporter, the last line for each case will contain two integers L and T, that it will be the last station the alien wants to go and the T number of stations she wants to visit as maximum.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span lang="en-US"><strong>OUTPUT</strong></span><span lang="en-US">:</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span lang="en-US"> The output will consists on P lines, each line containing the string "Scenario #i: " where i is the test case you're analyzing (starting by 1), followed by the minimum stations visited by the Alien to reach her destination, if she can't reach her destination on maximum T stations, print -1.</span></p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">&nbsp;</p>
<table style="width: 577px;" border="0" cellspacing="0" cellpadding="7">
<colgroup><col width="273"> <col width="274"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0in;" width="273">
<p lang="en-US" align="CENTER"><strong>INPUT</strong></p>
</td>
<td style="border: 1px solid #000000; padding: 0in 0.08in;" width="274">
<p lang="en-US" align="CENTER"><strong>OUTPUT</strong></p>
</td>
</tr>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0in;" width="273">
<p><span style="font-size: x-small;">4<br> </span></p>
<p><span style="font-size: x-small;">12 			6<br> 1 			3 4 1 2 -2<br> 10 			10<br> </span></p>
<p><span style="font-size: x-small;">12 			6<br> 1 			3 2 1 2 -2<br> 10 			10<br> </span></p>
<p><span style="font-size: x-small;">10 			2<br> 6 			-2<br> 5 			10<br> </span></p>
<p><span style="font-size: x-small;">10 			2<br> 1 			1<br> 10 			5</span></p>
</td>
<td style="border: 1px solid #000000; padding: 0in 0.08in;" width="274">
<p style="margin-bottom: 0in;"><span style="font-size: x-small;">Scenario #1: 4<br>Scenario #2:&nbsp;6<br>Scenario #3:&nbsp;3<br>Scenario #4:&nbsp;-1</span></p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">"Blank line between input sample data is just for clarification and understanding of the problem"</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">Explanation of the first test case:</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">She teleports from station 0 to station 4 using the third teleporter, from 4 to 7 using the second teleporter, from 7 to 9 using the fifth teleporter and she can either walk to the next station or use another teleporter.</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">Explanation of the last case:</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">She can't reach the station 10 going through only 5 stations, the answer should be then -1.</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span lang="en-US"><strong>CONSTRAINTS</strong></span><span lang="en-US">:</span></p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">1 &lt;= P &lt;= 50</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">1 &lt;= N &lt;= 100</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">1 &lt;= K &lt;= 17</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">-100 &lt;= Ki &lt;= 100</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">0 &lt;= L &lt;= N</p>
<p style="margin-bottom: 0in;" lang="en-US" align="JUSTIFY">1 &lt;= T &lt;= 50</p>