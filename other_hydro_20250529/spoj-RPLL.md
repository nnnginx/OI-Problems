<p>&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">&nbsp;German is the chief of the Rescuers and Principal Lifesavers of the ocean (RPL), he is in charge of commanding the search of survivors on a range given after a ship sinks, this range is established from the time that the ship sunk, he will always know this value, because he is magnificent in maths, however, he isn't good calculating the perfect searching range, this causes problem in rescuing survivors as the ship may exceed the limit of the area of searching.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> It is known that German will always send three ships to make the rescue effective, as he can't send all his ships, he wants to maximize the area of the three ships covers. The ships of German aren't sophisticated, so they will be going on a single direction (always) and a constant speed. The ships moves every unit of time.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> We say that an area is covered when the area made by the three points (triangular area) is lesser or equal than the maximum area that German knows.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> German will give you the initial coordinates of all three ships (given in 2D), the direction the ship will be going and the speed per hour. The direction of the rescuer ship will always be to north, south, east or west and the maximum area of search. Please have in count that the area covered by the three ships must NOT exceed the area that German gives to you.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>INPUT:</strong></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> The first line of the test data will start with an integer T representing the T test cases, then, T*4 Lines will follow, each of the following lines will contain, respectively, the maximum area of searching, the next three lines will contain, each, three integers and a string, denoting the coordinates the ship is in, the direction and the speed.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>OUTPUT:</strong></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> You must output the string ��Scenario #i: �� where i is the number of test case you're analyzing, followed by the time that </span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">the three ships will cover the maximum possible area (without exceeding it). Time will always be discrete.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<table style="width: 100%;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="128*"> <col width="128*"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0.04in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="CENTER"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>INPUT</strong></span></p>
</td>
<td style="border: 1px solid #000000; padding: 0.04in;" width="50%">
<p align="CENTER"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>OUTPUT</strong></span></p>
</td>
</tr>
<tr valign="TOP">
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">2</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">150</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">1 4 			north 2</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">2 0 			south 2</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">3 1 east 			2</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">12</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 -2 			north 1 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 0 			north 2</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 0 east 			3</span></p>
</td>
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in;" width="50%">
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Scenario 			#1: 5</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Scenario 			#2: 2</span></p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>CONSTRAINTS:</strong></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">1 &lt;= T &lt;= 100</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">-10^6 &lt;= X,Y &lt;= 10^6</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">1 &lt;= Speed &lt;= 10</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Small Input (30%)</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> For the ��small�� input, the triangles will always be rectangled triangles, making the area of them easier to calculate.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> 1 &lt;= Max_Area_Of_Searching &lt;= 10^3</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Large Input (70%)</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> Points will form any triangle, time-limit is heavier on these files.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> 10^3 &lt;= Max_Area_Of_Searching &lt;= 10^9</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Explanation of the second sample:</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">At hour two, the ship 1 will be at position (0,0), the ship 2 will be at position (0,4) and the ship 3 will be in (6,0), computing the area of a triangle, we will have a value of 12, as we know that there is no other possible area that satisfies the maximum without exceeding it, we output 2.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">It is guaranteed that all three ships will always be distancing themselves, then, the next area will always be bigger.</span></p>