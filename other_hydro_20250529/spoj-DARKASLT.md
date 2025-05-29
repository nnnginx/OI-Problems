<p style="margin-bottom: 0in; text-align: left;"><a href="https://docs.google.com/open?id=0B9MWHgzm3i0iUjdJdjVzYlVlUUU">Original statement</a></p>
<p style="margin-bottom: 0in; text-align: left;">Rainbowland is a planet full of life and adorable beings, however, this night, the spies Andreina, Marge and Teresa agreed to breakdown the security of a building led by a teddy bear, this teddy bear is mean! Don't get the wrong idea, the rainbowland spies agency (RSA) just want to make things go right in they colorful and lovable world.</p>
<p style="margin-bottom: 0in; text-align: left;">Andreina offered a plan to take control of the building, she and Teresa will go to the roof of another building, seeing the target building, they will tell Marge to take down N rivals on a building of F floors, as she won't use the stairs, there are a series of E elevators that are in the building, the elevator can only go up or down P floors (more explanation on input details).</p>
<p style="margin-bottom: 0in; text-align: left;">While Andreina and Teresa sees from outside, Marge must take down immediately the rivals, so they cannot leave them alive, otherwise, they will alert the others and the mission will be failed, when fighting a rival, the rival loses K points of life during each second using normal abilities, you can always assume that Marge won't fail at any fight, in addition, Marge can use some special abilities, these abilities allow Marge to deliver powerful blows, however, these special abilities can only be used <strong>once</strong>, so she must use it wisely, as Marge doesn't want to waste energy on a single enemy, she will give two special ability punches at most, if she can do it. She can always combine, so at last, she will choose between what is best (If normal attacking, if using one special ability or two and normal attacking).</p>
<p style="margin-bottom: 0in; text-align: left;">Help the spies Andreina, Teresa and Marge to find the minimum time so they can take the building and defeat all the rivals, having in consideration that:</p>
<ol style="text-align: left;">
<li>
<p style="margin-bottom: 0in;" align="LEFT">Marge takes one minute 	to use the elevator.</p>
</li>
<li>
<p style="margin-bottom: 0in;" align="LEFT">Each round of fight 	lasts one minute.</p>
</li>
<li>
<p style="margin-bottom: 0in;" align="LEFT">Marge starts from floor 	1 and she can go from floor 1 to F, never lower nor higher.</p>
</li>
<li>
<p style="margin-bottom: 0in;" align="LEFT">If Marge uses an 	special ability or two special abilities, it will still count as she 	uses on one round (see point 2).</p>
</li>
<li>
<p style="margin-bottom: 0in;" align="LEFT"><em>There will be <strong>from 	1 to</strong> <strong>7</strong> rivals in all the building.</em></p>
</li>
<li>
<p style="margin-bottom: 0in;" align="LEFT">The 	floor 1 will be always rival free, therefore, the <strong>floor 1</strong> will have a value of zero (0).</p>
</li>
</ol>
<p style="margin-bottom: 0in; text-align: left;">&nbsp;</p>
<p style="margin-bottom: 0in; text-align: left;"><strong>INPUT DETAILS:</strong></p>
<p style="margin-bottom: 0in; text-align: left;">First line will contain an integer T denoting T description of the test cases.</p>
<p style="margin-bottom: 0in; text-align: left;">For each T you will have four integers F, N, K, E denoting, respectively, the number of floors in the building, the number of special ability that Marge can use, the damage K that Marge delivers after a single blow and the number E of elevators.</p>
<p style="margin-bottom: 0in; text-align: left;">Then, in the next line, F integers separated by a single space will follow, denoting the description of the building, a number 0 means that there are no rivals at the floor, a positive number will represent the life points that the rival has at the moment of the assault.</p>
<p style="margin-bottom: 0in; text-align: left;">The next line will contain N integers separated by a single space representing the values of a special blow given by Marge, remember that she can only deliver two blows at most for each rivals and she can use only once the special blow.</p>
<p style="margin-bottom: 0in; text-align: left;">The next line will contain E integers separated by a single space, meaning the description of the elevators, for each positive number means that the elevator will go up P floors, if the number is negative, means that the elevator will go down P floors, you can always asume that P will never be 0.</p>
<p style="margin-bottom: 0in; text-align: left;">&nbsp;</p>
<p style="margin-bottom: 0in; text-align: left;"><strong>OUTPUT DETAILS:</strong></p>
<p style="margin-bottom: 0in; text-align: left;">For each test case, print the string ��Scenario #i: V�� where i denotes the i-th test case you're analyzing (starting from 1) and V is the minimum time that the team can defeat the all rivals, print -1 if the mission will fail.</p>
<p style="margin-bottom: 0in; text-align: left;">&nbsp;</p>
<p style="margin-bottom: 0in; text-align: left;">&nbsp;</p>
<p style="margin-bottom: 0in; text-align: left;">&nbsp;</p>
<table style="width: 100%; text-align: left;" border="0" cellspacing="0" cellpadding="4">
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
<p align="LEFT">3</p>
<p align="LEFT">4 2 3 2</p>
<p align="LEFT">0 10 0 15</p>
<p align="LEFT">10 5</p>
<p align="LEFT">2 -1</p>
<p align="LEFT">10 4 2 5</p>
<p align="LEFT">0 0 0 10 0 8 7 8 10 100</p>
<p align="LEFT">10 10 10 80</p>
<p align="LEFT">2 -1 5 -3 1</p>
<p align="LEFT">3 3 2 1</p>
<p align="LEFT">0 100 100</p>
<p align="LEFT">150 200 150</p>
<p align="LEFT">2</p>
</td>
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in;" width="50%">
<p align="LEFT">Scenario #1: 8</p>
<p align="LEFT">Scenario #2: 26</p>
<p align="LEFT">Scenario #3: -1</p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in; text-align: left;">&nbsp;</p>
<p style="margin-bottom: 0in; text-align: left;"><strong>Explanation of the first test case:</strong></p>
<p style="margin-bottom: 0in; text-align: left;">At time <strong>1</strong>, Marge goes from floor 1 to floor 3, then, from floor 3 to floor 2, she choose to beat the rival with life 10 with normal blows (it will take <strong>4</strong> units of time to beat it), at this time Marge has already wasted <strong>6</strong> minutes of time, then, she will take the elevator up to floor 4, then will use her two special abilities to deliver a powerful blow on rival at floor 4 with 15 life points (15-10-5 = 0) beating it. Final time of the mission, <strong>8</strong>.</p>
<p style="margin-bottom: 0in; text-align: left;">&nbsp;</p>
<p style="margin-bottom: 0in; text-align: left;"><strong>CONSTRAINTS:</strong></p>
<p style="margin-bottom: 0in; text-align: left;">&nbsp;</p>
<p style="margin-bottom: 0in; text-align: left;">1&lt;=T&lt;=10</p>
<p style="margin-bottom: 0in; text-align: left;">2&lt;=F&lt;=128</p>
<p style="margin-bottom: 0in; text-align: left;">1&lt;=N&lt;=7</p>
<p style="margin-bottom: 0in; text-align: left;">1&lt;=K&lt;=1000</p>
<p style="margin-bottom: 0in; text-align: left;">1&lt;=E&lt;=50</p>
<p style="margin-bottom: 0in; text-align: left;">0&lt;=Fi&lt;=1000</p>
<p style="margin-bottom: 0in; text-align: left;">1&lt;=Ni&lt;=1000</p>
<p style="margin-bottom: 0in; text-align: left;">-F&lt;=Ei&lt;=F with Ei != 0</p>
<p style="margin-bottom: 0in; text-align: left;">&nbsp;</p>
<p style="margin-bottom: 0in; text-align: left;"><strong>Clarification: There is no blank lines between Scenarios in the output.</strong></p>