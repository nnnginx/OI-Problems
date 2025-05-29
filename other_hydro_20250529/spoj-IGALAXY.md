<p><a href="https://docs.google.com/open?id=0B9MWHgzm3i0ib3pPYzNZS0txVjA"> </a></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-family: arial, helvetica, sans-serif;"><a href="https://docs.google.com/open?id=0B9MWHgzm3i0iMzk4UWFONk9uVkU"><span style="font-size: small;">ORIGINAL STATEMENT</span><span style="font-size: small;">&nbsp;</span></a></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> The world is on constant evolution, the humans evolved to a galactic civilization at the year 700,000, they are now capable of going instantly to any other planet in 1 unit of time, however, they must stop sometimes in a planet to avoid a horrible collision against an asteroid.</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> Rudolph-X3000, a single humanoid, wants to visit his family visiting as fewer planet as possible from planet A to planet B inclusive without repeating any planet, he is in a hurry so he need the answer quickly. Can you determine how many planets is going to visit?</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> As Rudolph-X3000 is an intergalactic traveler, he want to determine the planets he is going to visit as well, if there exists more than a single shortest path between planet A and B, print the one lexicographically smallest, if there isn't exists such route, print -1.</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> The human race knows now the Delta Velocity, this velocity allows to move in a single unit of time at a very fast speed from a place i to place j. So you can consider the distance between planets will be always of 1.</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> <strong>INPUT</strong>:</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> The first line will contain an integer T representing T test cases</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> Then, in the next line, there will be an integer R denoting the number of relations between planet, a relation is considered so that from a planet i you can go to planet j, this relation is symmetric, so the path between (i,j) is the same as (j,i)</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> The next R lines will contain two strings P and Q, these strings will denote the name of a planet P and a name of a planet Q and their relation.</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> The last line will contain two strings S and D, representing the origin planet and the destiny planet.</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;">Note: All the strings will have the combination of uppercase and lowercase letters [A-Z] [a-z].</span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> <strong>OUTPUT</strong>:</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;"> For each test case you shall print the string ��Scenario #i: �� where i is the test case you're analyzing (starting from 1) followed by the minimum number of planets, then, in the next line, you should list each planet visit (including origin and destiny), each one separated by a single space.</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><strong><span style="font-family: arial, helvetica, sans-serif;">SAMPLE CASE:</span></strong></p>
<table style="width: 100%;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="128*"> <col width="128*"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0.04in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="CENTER"><span style="font-size: small;"><strong><span style="font-family: arial, helvetica, sans-serif;">INPUT</span></strong></span></p>
</td>
<td style="border: 1px solid #000000; padding: 0.04in;" width="50%">
<p align="CENTER"><span style="font-size: small;"><strong><span style="font-family: arial, helvetica, sans-serif;">OUTPUT</span></strong></span></p>
</td>
</tr>
<tr valign="TOP">
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">3</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">8</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Mercury Venus</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Venus Earth</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Earth Mars</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Mars Jupiter</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Jupiter Saturn</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Saturn Uranus</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Uranus Neptune</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Neptune Pluto</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Earth Pluto</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">7</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Mesopotamia Merrick</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Merian Earth</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Earth Venus</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Merian Merrick</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Venus Mesopotamia</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Pluto Earth</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Mesopotamia Pluto</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Mesopotamia Earth</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">2</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Earth Sun</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Moon Venus</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Earth Moon</span></span></p>
</td>
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in;" width="50%">
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Scenario #1: 7</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Earth Mars Jupiter Saturn Uranus 			Neptune Pluto</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Scenario #2: 3</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Mesopotamia Pluto Earth</span></span></p>
<p align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Scenario #3: -1</span></span></p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">Explanation of the second case:</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">There are two possible routes for going from Mesopotamia to Earth, one is ��Mesopotamia �� Pluto �� Earth��, the other one is ��Mesopotamia �� Venus �� Earth��, we select the lexicographically smaller.</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">CONSTRAINTS:</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">1&lt;=T&lt;=100</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">1&lt;=R&lt;=100,000</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">1&lt;=|{P.Q.S.D}|&lt;=50</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">&nbsp;</span></span></p>
<p style="margin-bottom: 0in;" align="LEFT"><span style="font-size: small;"><span style="font-family: arial, helvetica, sans-serif;">It is safe to say that there will be no more than 10,000 distinct planets.</span></span></p>