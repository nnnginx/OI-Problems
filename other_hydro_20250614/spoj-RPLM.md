<p>&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">&nbsp;Charlie is picking some precious stones in a cave, this cave is known worldwide by the stones in it, however, this cave is very delicate and the minimum movement causes an instant collapse, Charlie knows the times that the tunnels will be free (as the instant collapses can free some tunnels) or covered by a pile of stones.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> In his backpack, Charlie has some magical hammers that he carries for emergency, in some expeditions he won't have these hammers, but in others he will. The hammer causes an instant opening of any pile of stones blocking his way.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> It is also known that Charlie travels some distance <strong>d</strong> in a time <strong>t</strong> from room <strong>i</strong> to room <strong>j</strong>, and the tunnel connecting them will be free from time <strong>x</strong> to time <strong>y</strong>. Charlie can return whenever he wants, so, traveling from room <strong>j</strong> to room <strong>i</strong> will be symmetric.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> Charlie doesn't have infinite hammers, so, when he use one, the hammer will break, making it useless.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> In addition, if Charlie knows that the tunnel will open in a time X, he can choose to stay until the path opens or use a magical hammer to go through the tunnel.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> Given that information, your task is to find the minimum time with the minimum distance that Charlie can go from the entrance (0) to the center of the cave (V-1)</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>INPUT:</strong></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> The first line of the test data will start with an integer T representing the T test cases, then, T cases will follow, each of the cases starts with three integers, V E and M, denoting, respectively, the number of the rooms on the cave, the numbers of tunnels in the cave and the number of hammers Charlie will carry, the next E lines will contain six integers, denoting, respectively, the origin room <strong>i</strong>, the destiny room <strong>j</strong>, opening time <strong>x</strong>, collapse time <strong>y</strong>, distance <strong>z</strong>, and time <strong>t</strong>.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>OUTPUT:</strong></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> You must output the string ��Scenario #i: �� where i is the number of test case you're analyzing, followed by the minimum time and the minimum distance associated to it, if Charlie isn't able to arrive to the V-1 room, output -1.</span></p>
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
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">4 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">6 6 2 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 1 1 18 			3 3 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 2 1 12 			4 4 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 4 1 3 			5 5 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">2 3 1 8 			2 2 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">3 4 1 5 			3 3 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">4 5 5 20 			1 1 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">6 6 1 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 1 1 18 			3 3 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 2 1 12 			4 4 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 4 1 3 			5 5 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">2 3 1 8 			2 2 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">3 4 1 5 			3 3 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">4 5 5 20 			1 1 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">6 6 0 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 1 1 18 			3 3 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 2 1 12 			4 4 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 4 1 3 			5 5 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">2 3 1 8 			2 2 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">3 4 8 25 			3 3 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">4 5 5 20 			1 1 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">3 3 0 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 1 0 5 			4 4 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">1 2 0 5 			2 2 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">0 2 0 5 			6 6</span></p>
</td>
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in;" width="50%">
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Scenario 			#1: 6 6 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Scenario 			#2: 7 6 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Scenario 			#3: 12 10 </span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Scenario 			#4: -1</span></p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>CONSTRAINTS:</strong></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">1 &lt;= T &lt;= 10</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Small input: (20%)</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> 2 &lt;= V &lt;= 10</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> 1 &lt;= E &lt;= 30</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> M = 0</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Medium input: (30%)</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> 2 &lt;= V &lt;= 100</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> 1 &lt;= E &lt;= 1,000</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> M = 0</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Large input: (50%)</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> 2 &lt;= V &lt;= 100</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> 1 &lt;= E &lt;= 1,000</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> 0 &lt;= M &lt;= 50</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">It is guaranteed that the distance of the tunnels won't never exceed 10.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">1 &lt;= opening and collapse times &lt;= 100,000</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><strong>Clarifications: </strong>You start with time 0. It will be always true that the time x will be lesser or equal than time y. While passing through a tunnel from room i to room j, if the tunnel collapses while you're inside, you can use a hammer to break through, otherwise that path is impossible to take.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><br></span></p>